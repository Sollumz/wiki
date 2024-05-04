---
description: >-
  Game Collisions are stored in the Static Collisions (.ybn) file format.
  Creating Collisions in Sollumz is very straight forwards.
---

# 💥 Creating Static Collisions

### Prerequisite Knowledge

* Basic Blender skills ([This is a great place to start](https://www.youtube.com/playlist?list=PLjEaoINr3zgFX8ZsChQVQsuDSjEqdWMAD))
* Know how to either stream assets in a FiveM server or load mods into the base-game

### What you will need

* A mesh located at the world location (where you want the collision to be)

### Converting to a Static Collision

The first thing to do is apply location transforms on your object(s). Select all the objects and press CTRL + A and select 'Location'.

&#x20;Next go to Sollumz Tools > Collisions > Create Bounds and select your object(s) and click 'Convert to Composite'.

&#x20;                                             ![](<../.gitbook/assets/image (1).png>)

&#x20;Ensure that the Bound Composite and Bound GeometryBVH empties are located at 0, 0, 0.

&#x20;Next, Center the origins of your object(s), go to Object > Set Origin > Origin to Geometry.&#x20;

<figure><img src="../.gitbook/assets/image.png" alt=""><figcaption><p>Example Hierarchy</p></figcaption></figure>

&#x20;                                                    It should now look something like this.

&#x20;                                                    <img src="../.gitbook/assets/image (4).png" alt="" data-size="original">&#x20;

Last step is to rename the 'Bound Composite' empty to your .ybn file name.

### Additional tips

Using Primitive shapes such as, 'Bound Poly Box', 'Bound Poly Capsule', 'Bound Poly Sphere' should be used for majority of your collisions, unless the mesh is a complex shape and cannot be made up of multiple primitive shapes. This is because it is more performance friendly and reduces unnecessary asset size.
