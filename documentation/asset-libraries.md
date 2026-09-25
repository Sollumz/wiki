# 📚 Asset Libraries

An asset library is a folder of `.blend` files, marked up as Blender assets, that mirrors the props defined in a set of YTYPs. Sollumz builds them once from your game install (or from a folder of extracted files), and from then on:

* props appear in Blender's **Asset Browser**, organised into catalogs, ready to drag into a map;
* importing a YMAP or a YTYP MLO **instances** archetypes straight from the library instead of failing on missing models;
* features like LOD light baking and entity LOD-distance resolution read the metadata baked into the assets, so they work without ever touching the original game files again.

<figure><img src="../.gitbook/assets/asset_library_highlight.png" alt=""><figcaption><p>An asset library</p></figcaption></figure>

Building a library from a full GTA V installation takes a long time and produces a lot of data — it is a one-off setup step, not something you re-run per project.

### Before you start: configure a Shared Assets directory

Libraries are written into a **Shared Assets directory**, configured in `Edit → Preferences → Add-ons → Sollumz`. Without one, **Build Asset Library** refuses to run:

> No Shared Assets directory configured. Add one in Preferences > Sollumz.

Each entry has a **Name** and a **Path**, and the list is ordered — use the up/down arrows to set search priority. You can add a directory from the preferences, or on the fly from the build dialog (see **New…** below).

{% hint style="info" %}
Register the same directory as a **Blender asset library** (`Preferences → File Paths → Asset Libraries`) so the props also show up in the Asset Browser. The Shared Assets list tells Sollumz where to write and where to look up; Blender's own list is what populates the browser.
{% endhint %}

<figure><img src="../.gitbook/assets/image (118).png" alt="" width="548"><figcaption><p>Asset Library panel</p></figcaption></figure>

| Button                          | Purpose                                                                                                 |
| ------------------------------- | ------------------------------------------------------------------------------------------------------- |
| **Import To Asset Library**     | Import drawables or fragments into the **current** `.blend` as marked assets, instead of into the scene |
| **Build Asset Library**         | Scan a directory of game files and generate `.blend` libraries in a Shared Assets directory             |
| **Debug - Rebuild Asset Cache** | Re-index the existing `.blend` libraries without re-importing anything                                  |

### Import To Asset Library

The ordinary Sollumz import dialog with _import as asset_ enabled. Use it to add a handful of props to the file you are working in — your own models, or a few vanilla props you want on hand. It does not write to a Shared Assets directory and does not update the cache.

For anything larger, use Build Asset Library.

### Build Asset Library

Press the button, pick the **source directory** in the file browser, and set the options in the sidebar before confirming.

The source can be either:

* **a GTA V installation** — detected by the presence of `GTA5.exe` or `GTA5_Enhanced.exe` at the root. Files inside RPF archives are read directly; no extraction needed. DLC load order is honoured, so when several packs define the same file the highest-priority one wins;
* **any folder of extracted assets** — scanned recursively for `*.ytyp` / `*.ytyp.xml`.

This operator parallelizes the work across multiple Blender background processes, significantly speeding up the build. Libraries are managed from the add-on preferences and integrate with Blender's asset browser.

<figure><img src="../.gitbook/assets/image (131).png" alt=""><figcaption></figcaption></figure>

#### Options

| Option              | Default          | What it does                                                                                                                        |
| ------------------- | ---------------- | ----------------------------------------------------------------------------------------------------------------------------------- |
| **Output Library**  | first configured | Which Shared Assets directory receives the `.blend` files. Choose **New…** to create one on the spot.                               |
| **Name** / **Path** | —                | Shown only when **New…** is selected: the name and location of the new directory, which is added to your preferences automatically. |
| **Pattern**         | empty            | **Regular expression** matched against YTYP names (without extension). Empty imports everything.                                    |
| **Subprocesses**    | `cpu_count / 4`  | Number of background Blender instances doing the work in parallel.                                                                  |

{% hint style="warning" %}
**Pattern is a regex, not a glob.** It uses Python `re` syntax with `search`, so it matches anywhere in the name and is **case-sensitive**. `v_int` matches every `v_int_*` YTYP; `^v_fastfood$` matches exactly one; `*.ytyp` is not valid and will error.
{% endhint %}

**Subprocesses** trades memory for speed. Each worker is a full headless Blender importing models and packing textures, so budget a few GB each. The default of a quarter of your cores is conservative; raising it to half is usually safe on a machine with plenty of RAM, and the maximum is your core count.

When instancing entities from YMAPs or YTYP MLOs, archetypes are resolved from these libraries, after first checking the current .blend. Assets built by Sollumz also embed metadata, allowing features like LOD light baking and entity LOD distance resolution to work without loading the original game files.

### Troubleshooting

**"Cannot build library on this Blender version. Update to Blender 4.2 or newer."** The build spawns workers through Blender CLI commands that only exist from 4.2.

**"No Shared Assets directory configured."** Add one in `Preferences → Add-ons → Sollumz`, or pick **New…** in the build dialog.

**"No .ytyp files found in '...'"** Either the source really contains no YTYPs, or your **Pattern** filtered them all out. Remember it is a case-sensitive regex.

**Console warning: "Asset cache not found … Run 'Build Asset Library' or 'Rebuild Asset Cache' first."** Nothing has been indexed yet. Instancing is skipped entirely until the cache exists.

**Console warning: "Asset cache is corrupted or has wrong schema"** Run **Debug - Rebuild Asset Cache**.

**`not found <path>` printed during a build** A YTYP references an asset or texture dictionary that is not present in the source directory. Common when building from a partial extraction rather than a full install.

**Props import but the Asset Browser stays empty** The output directory is registered as a Sollumz Shared Assets directory but not as a Blender asset library. Add it in `Preferences → File Paths → Asset Libraries`.

**"No output library selected; using the first configured directory."** Several directories are configured and the dialog's choice did not resolve. Harmless, but check that the files landed where you expected.

### Requirements

Blender 4.2 or newer for **Build Asset Library**. The other operators have no version floor beyond Sollumz's own.
