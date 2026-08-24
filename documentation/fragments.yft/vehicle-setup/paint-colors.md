# Paint Colors

Paint layers determine which of the vehicle's paint colors a material is tinted with in-game: the **Primary** color, **Secondary** color, **Pearlescent** color, **Wheel** color, **Interior Trim** color or **Dashboard** color. To select the paint layer for a material, select the mesh object, then navigate to `Material Properties > Sollumz > Fragment (Vehicle Paint)`.

<figure><img src="../../../.gitbook/assets/image (127).png" alt="" width="563"><figcaption><p>Material Properties > Sollumz > Fragment (Vehicle Paint)</p></figcaption></figure>

This panel only appears on materials that use a `VEHICLE` shader.

<table><thead><tr><th width="228">Paint Layer</th><th width="472">Description</th></tr></thead><tbody><tr><td><code>Custom - Not Paintable</code></td><td>Cannot be painted at mod shops. The <code>matDiffuseColor</code> parameter is used as the paint color RGB values.</td></tr><tr><td><code>Default - Not Paintable</code></td><td>Cannot be painted at mod shops. White is used as the paint color, or grey when the vehicle is scorched.</td></tr><tr><td><code>Primary</code></td><td>Use the Primary paint color.</td></tr><tr><td><code>Secondary</code></td><td>Use the Secondary paint color.</td></tr><tr><td><code>Pearlescent</code></td><td>Use the Pearlescent paint color. Note this does not apply the pearlescent effect, it simply paints the material with the pearlescent color.</td></tr><tr><td><code>Wheel</code></td><td>Use the Wheel paint color.</td></tr><tr><td><code>Interior Trim</code></td><td>Use the Interior Trim paint color.</td></tr><tr><td><code>Dashboard</code></td><td>Use the Interior Dashboard paint color.</td></tr></tbody></table>

The paint layer is not stored as a separate parameter, it is just a friendly way of setting the material's `matDiffuseColor` value parameter, which is what the game actually reads.

When you choose a paint layer, Sollumz appends it to the material name (for example `vehicle_paint1 [PRIMARY]`) so you can tell at a glance how each material will be painted. `Custom` and `Default` add no suffix.

{% hint style="info" %}
Not all vehicle shaders are paintable. If you are trying to set up a paintable vehicle material and the paint layer selector is greyed out with the "Not a vehicle paint shader. Shader must have a matDiffuseColor parameter." message, then you need to use a different shader. Typically you'd want to use a `vehicle_paint` shader for the body of a vehicle.
{% endhint %}

#### Previewing paint colors

To see what the paint layers look like in the viewport, select the Fragment root object and navigate to `Object Properties > Sollumz > Vehicle Render Preview`. There is a color picker for each paint layer, along with dirt and light emissive settings.

These colors only affect how the vehicle looks in Blender's Material Preview and Rendered viewport shading modes. They are not exported and have no effect in-game.

<figure><img src="../../../.gitbook/assets/image (126).png" alt=""><figcaption><p>Paint colors in Vehicle Render Preview</p></figcaption></figure>
