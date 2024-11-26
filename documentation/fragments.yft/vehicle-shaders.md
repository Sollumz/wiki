---
description: >-
  In this page you can find all vehicle shaders used on vehicles and their
  technical usage
---

# Vehicle Shaders

### Vehicle Paint shaders

`vehicle_paint1`

{% tabs %}
{% tab title="📚 Description" %}
Typical vehicle paint shader, used on most vehicles in GTA V.
{% endtab %}

{% tab title="🎨 Texture Sampler(s)" %}
* [x] Diffuse
* [x] Dirt
* [x] Specular
{% endtab %}

{% tab title="🗺 UV Maps" %}
<table><thead><tr><th width="205">UV Maps</th><th width="494">Texture</th></tr></thead><tbody><tr><td>UVMap 0</td><td>Diffuse / Specular</td></tr><tr><td>UVMap 1 </td><td>Dirt</td></tr></tbody></table>
{% endtab %}

{% tab title="✒ Example" %}
<figure><img src="../../.gitbook/assets/obraz (1).png" alt=""><figcaption><p>Example of vehicle_paint1 in blista.yft</p></figcaption></figure>
{% endtab %}
{% endtabs %}

***

`vehicle_paint1_enveff`

{% tabs %}
{% tab title="📚 Description" %}
Basic vehicle paint shader with additional feature of applying snow.

Vertex Alpha: visibility of snow samplers (**black** - non applied, **white** - applied)
{% endtab %}

{% tab title="🎨 Texture Sampler(s)" %}
* [x] Diffuse
* [x] Snow sampler 0
* [x] Snow sampler 1
* [x] Dirt
* [x] Specular
{% endtab %}

{% tab title="🗺 UV Maps" %}
<table><thead><tr><th width="320">UV Maps</th><th width="379">Texture</th></tr></thead><tbody><tr><td>UVMap 0</td><td>Diffuse / Specular</td></tr><tr><td>UVMap 1 </td><td>Dirt</td></tr></tbody></table>
{% endtab %}

{% tab title="✒ Example" %}
<figure><img src="../../.gitbook/assets/obraz (9).png" alt=""><figcaption><p>Example of vehicle_paint1_enveff from asea2.yft</p></figcaption></figure>
{% endtab %}
{% endtabs %}

***

`vehicle_paint2`

{% tabs %}
{% tab title="📚 Description" %}
A very similar shader to vehicle\_paint1, with dirt mapping moved to first UV map.
{% endtab %}

{% tab title="🎨 Texture Sampler(s)" %}
* [x] Diffuse
* [x] Dirt
* [x] Specular
{% endtab %}

{% tab title="🗺 UV Maps" %}
<table><thead><tr><th width="321">UV Maps</th><th width="379">Texture</th></tr></thead><tbody><tr><td>UVMap 0</td><td>Diffuse / Specular / Dirt</td></tr></tbody></table>
{% endtab %}

{% tab title="✒ Example" %}
<figure><img src="../../.gitbook/assets/obraz (2).png" alt=""><figcaption><p>Example of vehicle_paint2 from burrito3.yft</p></figcaption></figure>
{% endtab %}
{% endtabs %}

***

`vehicle_paint2_enveff`

{% tabs %}
{% tab title="📚 Description" %}
A copy of vehicle\_paint2 with additional feature of applying snow.

Vertex Alpha: visibility of snow samplers (**black** - non applied, **white** - applied)
{% endtab %}

{% tab title="🎨 Texture Sampler(s)" %}
* [x] Diffuse
* [x] Snow sampler 0
* [x] Snow sampler 1
* [x] Dirt
* [x] Specular
{% endtab %}

{% tab title="🗺 UV Maps" %}
<table><thead><tr><th width="321">UV Maps</th><th width="379">Texture</th></tr></thead><tbody><tr><td>UVMap 0</td><td>Diffuse / Specular / Dirt</td></tr></tbody></table>
{% endtab %}

{% tab title="✒ Example" %}
<figure><img src="../../.gitbook/assets/paint2_enveff.png" alt=""><figcaption><p>Example of converted material for vehicle_paint2_enveff</p></figcaption></figure>
{% endtab %}
{% endtabs %}

***

`vehicle_paint3`

{% tabs %}
{% tab title="📚 Description" %}
Used for liveries on a car.
{% endtab %}

{% tab title="🎨 Texture Sampler(s)" %}
* [x] Diffuse
* [x] Second diffuse
* [x] Dirt
* [x] Specular
{% endtab %}

{% tab title="🗺 UV Maps" %}
<table><thead><tr><th width="319">UV Maps</th><th width="379">Texture</th></tr></thead><tbody><tr><td>UVMap 0</td><td>Diffuse / Dirt</td></tr><tr><td>UVMap 1</td><td>Second diffuse / Specular</td></tr></tbody></table>
{% endtab %}

{% tab title="✒ Example" %}
<figure><img src="../../.gitbook/assets/obraz (6).png" alt=""><figcaption><p>Example of vehicle_paint3 from buffalo3.yft</p></figcaption></figure>
{% endtab %}
{% endtabs %}

***

`vehicle_paint3_enveff`

{% tabs %}
{% tab title="📚 Description" %}
A copy of vehicle\_paint3 with additional feature of applying snow.

Vertex Alpha: visibility of snow samplers (**black** - non applied, **white** - applied)
{% endtab %}

{% tab title="🎨 Texture Sampler(s)" %}
* [x] Diffuse
* [x] Snow sampler 0
* [x] Snow sampler 1
* [x] Second diffuse
* [x] Dirt
* [x] Specular
{% endtab %}

{% tab title="🗺 UV Maps" %}
<table><thead><tr><th width="319">UV Maps</th><th width="379">Texture</th></tr></thead><tbody><tr><td>UVMap 0</td><td>Diffuse / Dirt / Enveff tileable UV (edited in envEffTexTileUV)</td></tr><tr><td>UVMap 1</td><td>Second diffuse / Specular</td></tr></tbody></table>
{% endtab %}

{% tab title="✒ Example" %}
<figure><img src="../../.gitbook/assets/paint3_enveff.png" alt=""><figcaption><p>Example of vehicle_paint3_enveff from stunt.yft</p></figcaption></figure>
{% endtab %}
{% endtabs %}

***

`vehicle_paint3_lvr`

{% tabs %}
{% tab title="📚 Description" %}
Variant of vehicle\_paint3 with tileable livery via second UV Map.
{% endtab %}

{% tab title="🎨 Texture Sampler(s)" %}
* [x] Diffuse
* [x] Third diffuse
* [x] Dirt
* [x] Specular
{% endtab %}

{% tab title="🗺 UV Maps" %}
<table><thead><tr><th width="319">UV Maps</th><th width="379">Texture</th></tr></thead><tbody><tr><td>UVMap 0</td><td>Diffuse / Dirt</td></tr><tr><td>UVMap 1</td><td>Livery / Specular</td></tr></tbody></table>
{% endtab %}

{% tab title="✒ Example" %}
<figure><img src="../../.gitbook/assets/paint3_lvr.png" alt=""><figcaption><p>Example of vehicle_paint3_lvr from tornado5.yft</p></figcaption></figure>
{% endtab %}
{% endtabs %}

***

`vehicle_paint4`

{% tabs %}
{% tab title="📚 Description" %}
Used for metal worn effect and/or livery on a car.
{% endtab %}

{% tab title="🎨 Texture Sampler(s)" %}
* [x] Diffuse
* [x] Second diffuse
* [x] Dirt
* [x] Specular
{% endtab %}

{% tab title="🗺 UV Maps" %}
<table><thead><tr><th width="321">UV Maps</th><th width="379">Texture</th></tr></thead><tbody><tr><td>UVMap 0</td><td>Dirt / Diffuse tileable UV (edited in DiffuseTexTileUV)</td></tr><tr><td>UVMap 1</td><td>Tileable specular (edited in specTexTileUV)</td></tr></tbody></table>
{% endtab %}

{% tab title="✒ Example" %}
<figure><img src="../../.gitbook/assets/obraz (5).png" alt=""><figcaption><p>Example of vehicle_paint4 from banshee.yft</p></figcaption></figure>
{% endtab %}
{% endtabs %}

***

`vehicle_paint4_emissive`

{% tabs %}
{% tab title="📚 Description" %}
Very same vehicle\_paint4 shader with support of emissives.
{% endtab %}

{% tab title="🎨 Texture Sampler(s)" %}
* [x] Diffuse
* [x] Snow sampler 0
* [x] Snow sampler 1
* [x] Second diffuse
* [x] Dirt
* [x] Specular
{% endtab %}

{% tab title="🗺 UV Maps" %}
<table><thead><tr><th width="321">UV Maps</th><th width="379">Texture</th></tr></thead><tbody><tr><td>UVMap 0</td><td>Dirt / Diffuse tileable UV (edited in DiffuseTexTileUV)</td></tr><tr><td>UVMap 1</td><td>Tileable specular (edited in specTexTileUV)</td></tr></tbody></table>
{% endtab %}

{% tab title="✒ Example" %}
<figure><img src="../../.gitbook/assets/paint4_emissive.png" alt=""><figcaption><p>Example of vehicle_paint4_emissive from blimp3.yft</p></figcaption></figure>
{% endtab %}
{% endtabs %}

***

`vehicle_paint4_enveff`

{% tabs %}
{% tab title="📚 Description" %}
vehicle\_paint4 shader, used for metal worn effect and liveries on a car.

Vertex Alpha: visibility of snow samplers (**black** - non applied, **white** - applied)
{% endtab %}

{% tab title="🎨 Texture Sampler(s)" %}
* [x] Diffuse
* [x] Snow sampler 0
* [x] Snow sampler 1
* [x] Second diffuse
* [x] Dirt
* [x] Specular
{% endtab %}

{% tab title="🗺 UV Maps" %}
<table><thead><tr><th width="321">UV Maps</th><th width="379">Texture</th></tr></thead><tbody><tr><td>UVMap 0</td><td>Dirt / Diffuse tileable UV (edited in DiffuseTexTileUV)</td></tr><tr><td>UVMap 1</td><td>Tileable specular (edited in specTexTileUV)</td></tr></tbody></table>
{% endtab %}

{% tab title="✒ Example" %}
<figure><img src="../../.gitbook/assets/paint4_enveff.png" alt=""><figcaption><p>Example of vehicle_paint4_enveff from caddy3.yft</p></figcaption></figure>
{% endtab %}
{% endtabs %}

***

`vehicle_paint5_enveff`

{% tabs %}
{% tab title="📚 Description" %}
Used for metal worn effect and liveries on a car.

Vertex Alpha: visibility of snow samplers (**black** - non applied, **white** - applied)
{% endtab %}

{% tab title="🎨 Texture Sampler(s)" %}
* [x] Diffuse
* [x] Snow sampler 0
* [x] Snow sampler 1
* [x] Second diffuse
* [x] Dirt
* [x] Specular
{% endtab %}

{% tab title="🗺 UV Maps" %}
<table><thead><tr><th width="320">UV Maps</th><th width="379">Texture</th></tr></thead><tbody><tr><td>UVMap 0</td><td>Dirt / Diffuse tileable UV (edited in DiffuseTexTileUV)</td></tr><tr><td>UVMap 1 </td><td>Livery</td></tr></tbody></table>
{% endtab %}

{% tab title="✒ Example" %}
<figure><img src="../../.gitbook/assets/obraz (8).png" alt=""><figcaption><p>Example of vehicle_paint5_enveff from camper.yft</p></figcaption></figure>
{% endtab %}
{% endtabs %}

***

`vehicle_paint6`

{% tabs %}
{% tab title="📚 Description" %}
Used for metal bolts on planes, applying liveries, metal worn effect.
{% endtab %}

{% tab title="🎨 Texture Sampler(s)" %}
* [x] Diffuse
* [x] Second diffuse
* [x] Dirt
* [x] Normal map
* [x] Specular
{% endtab %}

{% tab title="🗺 UV Maps" %}
<table><thead><tr><th width="320">UV Maps</th><th width="379">Texture</th></tr></thead><tbody><tr><td>UVMap 0</td><td>Dirt / Diffuse tileable UV (edited in DiffuseTexTileUV)</td></tr><tr><td>UVMap 1 </td><td>Livery</td></tr></tbody></table>
{% endtab %}

{% tab title="✒ Example" %}
<figure><img src="../../.gitbook/assets/obraz (7).png" alt=""><figcaption><p>Example of vehicle_paint6 from utillitruck.yft</p></figcaption></figure>
{% endtab %}
{% endtabs %}

`vehicle_paint7`

{% tabs %}
{% tab title="📚 Description" %}
Used for metal worn effect and liveries on a car.
{% endtab %}

{% tab title="🎨 Texture Sampler(s)" %}
* [x] Diffuse
* [x] Second diffuse
* [x] Dirt
* [x] Specular
{% endtab %}

{% tab title="🗺 UV Maps" %}
<table><thead><tr><th width="320">UV Maps</th><th width="379">Texture</th></tr></thead><tbody><tr><td>UVMap 0</td><td>Dirt / Specular / Diffuse tileable UV (edited in DiffuseTexTileUV)</td></tr><tr><td>UVMap 1 </td><td>Livery</td></tr></tbody></table>
{% endtab %}

{% tab title="✒ Example" %}
<figure><img src="../../.gitbook/assets/paint7.png" alt=""><figcaption><p>Example of vehicle_paint7 from phantom2.yft</p></figcaption></figure>
{% endtab %}
{% endtabs %}

***

`vehicle_paint7_enveff`

{% tabs %}
{% tab title="📚 Description" %}
Used for metal worn effect and liveries on a car.

Vertex Alpha: visibility of snow samplers (**black** - non applied, **white** - applied)
{% endtab %}

{% tab title="🎨 Texture Sampler(s)" %}
* [x] Diffuse
* [x] Snow sampler 0
* [x] Snow sampler 1
* [x] Second diffuse
* [x] Dirt
* [x] Specular
{% endtab %}

{% tab title="🗺 UV Maps" %}
<table><thead><tr><th width="320">UV Maps</th><th width="379">Texture</th></tr></thead><tbody><tr><td>UVMap 0</td><td>Dirt / Diffuse tileable UV (edited in DiffuseTexTileUV)</td></tr><tr><td>UVMap 1 </td><td>Livery</td></tr></tbody></table>
{% endtab %}

{% tab title="✒ Example" %}
<figure><img src="../../.gitbook/assets/paint7_enveff.png" alt=""><figcaption><p>Example of vehicle_paint7_enveff from wastelander.yft</p></figcaption></figure>
{% endtab %}
{% endtabs %}

***

`vehicle_paint8`

{% tabs %}
{% tab title="📚 Description" %}
Used for metal worn effect and liveries on a car.

Vertex Alpha: visibility of snow samplers (**black** - non applied, **white** - applied)
{% endtab %}

{% tab title="🎨 Texture Sampler(s)" %}
* [x] Diffuse
* [x] Snow sampler 0
* [x] Snow sampler 1
* [x] Second diffuse
* [x] Dirt
* [x] Dirt normal map
* [x] Normal map
* [x] Specular
{% endtab %}

{% tab title="🗺 UV Maps" %}
<table><thead><tr><th width="320">UV Maps</th><th width="379">Texture</th></tr></thead><tbody><tr><td>UVMap 0</td><td>Dirt normal map</td></tr><tr><td>UVMap 1 </td><td>Diffuse tileable UV (edited in DiffuseTexTileUV) / Snow sampler tileable UV (edited in envEffTexTileUV)/ Livery / Specular</td></tr><tr><td>UVMap 2</td><td>Dirt</td></tr></tbody></table>
{% endtab %}

{% tab title="✒ Example" %}
<figure><img src="../../.gitbook/assets/paint8.png" alt=""><figcaption><p>Example of vehicle_paint8 from brutus.yft</p></figcaption></figure>
{% endtab %}
{% endtabs %}

***

`vehicle_paint9`

{% tabs %}
{% tab title="📚 Description" %}
Used for metal worn effect and liveries on a car.

Vertex Alpha: visibility of snow samplers (**black** - non applied, **white** - applied)
{% endtab %}

{% tab title="🎨 Texture Sampler(s)" %}
* [x] Diffuse
* [x] Snow sampler 0
* [x] Snow sampler 1
* [x] Second diffuse
* [x] Dirt
* [x] Dirt normal map
* [x] Normal map
* [x] Specular
{% endtab %}

{% tab title="🗺 UV Maps" %}
<table><thead><tr><th width="320">UV Maps</th><th width="379">Texture</th></tr></thead><tbody><tr><td>UVMap 0</td><td>Dirt normal map</td></tr><tr><td>UVMap 1 </td><td>Livery</td></tr><tr><td>UVMap 2</td><td>Dirt / Diffuse tileable UV (edited in DiffuseTexTileUV) / Snow sampler tileable UV (edited in envEffTexTileUV) / Specular</td></tr></tbody></table>
{% endtab %}

{% tab title="✒ Example" %}
<figure><img src="../../.gitbook/assets/paint9.png" alt=""><figcaption><p>Example of vehicle_paint9 from conada.yft</p></figcaption></figure>
{% endtab %}
{% endtabs %}

***

### Vehicle Light shaders

`vehicle_lightsmeissive`

{% tabs %}
{% tab title="📚 Description" %}
Allows the light to be lit.
{% endtab %}

{% tab title="🎨 Texture Sampler(s)" %}
* [x] Diffuse
* [x] Dirt
* [x] Specular
{% endtab %}

{% tab title="🗺 UV Maps" %}
<table><thead><tr><th width="319">UV Maps</th><th width="379">Texture</th></tr></thead><tbody><tr><td>UVMap 0</td><td>Diffuse / Specular</td></tr><tr><td>UVMap 1 </td><td>Dirt</td></tr></tbody></table>
{% endtab %}

{% tab title="✒ Example" %}
<figure><img src="../../.gitbook/assets/obraz (11).png" alt=""><figcaption><p>Example of vehicle_lightsemissive from asea2.yft</p></figcaption></figure>
{% endtab %}
{% endtabs %}



Lights ID values for different type of vehicle lights, available in Fragments / Vehicle Light IDs

<figure><img src="../../.gitbook/assets/obraz (12).png" alt=""><figcaption><p>Lights ID</p></figcaption></figure>

***

### Vehicle Glass shaders

`vehicle_vehglass`

{% tabs %}
{% tab title="📚 Description" %}
Shader specifically tailored to work with windows and other glasses.
{% endtab %}

{% tab title="🎨 Texture Sampler(s)" %}
* [x] Diffuse
* [x] Dirt
* [x] Specular
{% endtab %}

{% tab title="🗺 UV Maps" %}
<table><thead><tr><th width="320">UV Maps</th><th width="379">Texture</th></tr></thead><tbody><tr><td>UVMap 0</td><td>Diffuse /  Specular</td></tr><tr><td>UVMap 1</td><td>Dirt</td></tr></tbody></table>
{% endtab %}

{% tab title="✒ Example" %}
<figure><img src="../../.gitbook/assets/vehglass.png" alt=""><figcaption><p>Example of vehicle_vehglass from buffalo2.yft</p></figcaption></figure>
{% endtab %}
{% endtabs %}

***

`vehicle_vehglass_inner`

{% tabs %}
{% tab title="📚 Description" %}
Identical shader to vehicle\_vehglass, used for inner side of windows/glasses, with limited dirt intensity.
{% endtab %}

{% tab title="🎨 Texture Sampler(s)" %}
* [x] Diffuse
* [x] Dirt
* [x] Specular
{% endtab %}

{% tab title="🗺 UV Maps" %}
<table><thead><tr><th width="320">UV Maps</th><th width="379">Texture</th></tr></thead><tbody><tr><td>UVMap 0</td><td>Diffuse /  Specular</td></tr><tr><td>UVMap 1</td><td>Dirt</td></tr></tbody></table>
{% endtab %}

{% tab title="✒ Example" %}
<figure><img src="../../.gitbook/assets/vehglass_inner.png" alt=""><figcaption><p>Example of vehicle_vehglass_inner from buffalo2.yft</p></figcaption></figure>
{% endtab %}
{% endtabs %}

***

### Vehicle Interior shaders

`vehicle_interior`

{% tabs %}
{% tab title="📚 Description" %}
Simple interior shader with normal map support.
{% endtab %}

{% tab title="🎨 Texture Sampler(s)" %}
* [x] Diffuse
* [x] Normal map
* [x] Specular
{% endtab %}

{% tab title="🗺 UV Maps" %}
<table><thead><tr><th width="321">UV Maps</th><th width="379">Texture</th></tr></thead><tbody><tr><td>UVMap 0</td><td>Diffuse / Normal map / Specular</td></tr></tbody></table>
{% endtab %}

{% tab title="✒ Example" %}
<figure><img src="../../.gitbook/assets/obraz (20).png" alt=""><figcaption><p>Example of vehicle_interior from vigero.yft</p></figcaption></figure>
{% endtab %}
{% endtabs %}

***

`vehicle_interior2`

Simple interior shader without normal map support.

{% tabs %}
{% tab title="📚 Description" %}
Simple interior shader without normal map support.
{% endtab %}

{% tab title="🎨 Texture Sampler(s)" %}
* [x] Diffuse
* [x] Specular
{% endtab %}

{% tab title="🗺 UV Maps" %}
<table><thead><tr><th width="320">UV Maps</th><th width="379">Texture</th></tr></thead><tbody><tr><td>UVMap 0</td><td>Diffuse /  Specular</td></tr></tbody></table>
{% endtab %}

{% tab title="✒ Example" %}
<figure><img src="../../.gitbook/assets/obraz (18).png" alt=""><figcaption><p>Example of vehicle_interior2 from burrito3.yft</p></figcaption></figure>
{% endtab %}
{% endtabs %}

***

### Vehicle Mesh shaders

`vehicle_mesh`

{% tabs %}
{% tab title="📚 Description" %}
Extensively used for metallic vehicle parts, like exhausts, engines, chassis parts.
{% endtab %}

{% tab title="🎨 Texture Sampler(s)" %}
* [x] Diffuse
* [x] Dirt
* [x] Normal map
* [x] Specular
{% endtab %}

{% tab title="🗺 UV Maps" %}
<table><thead><tr><th width="321">UV Maps</th><th width="379">Texture</th></tr></thead><tbody><tr><td>UVMap 0</td><td>Diffuse /  Normal map / Specular</td></tr><tr><td>UVMap 1</td><td>Dirt</td></tr></tbody></table>
{% endtab %}

{% tab title="✒ Example" %}
<figure><img src="../../.gitbook/assets/obraz (21).png" alt=""><figcaption><p>Example of vehicle_mesh from vigero.yft</p></figcaption></figure>
{% endtab %}
{% endtabs %}

***

`vehicle_mesh_enveff`

{% tabs %}
{% tab title="📚 Description" %}
Extensively used for metallic vehicle parts, like exhausts, engines, chassis parts with additional feature of applying snow.

Vertex Alpha: visibility of snow samplers (**black** - non applied, **white** - applied)
{% endtab %}

{% tab title="🎨 Texture Sampler(s)" %}

{% endtab %}

{% tab title="🗺 UV Maps" %}

{% endtab %}

{% tab title="✒ Example" %}

{% endtab %}
{% endtabs %}

***

### Vehicle Tire shaders

`vehicle_tire`

{% tabs %}
{% tab title="📚 Description" %}
A shader for wheels, **cannot be used** on any other vehicle parts.
{% endtab %}

{% tab title="🎨 Texture Sampler(s)" %}
* [x] Diffuse
* [x] Dirt
* [x] Normal map
* [x] Specular
{% endtab %}

{% tab title="🗺 UV Maps" %}
<table><thead><tr><th width="321">UV Maps</th><th width="379">Texture</th></tr></thead><tbody><tr><td>UVMap 0</td><td>Diffuse /  Dirt / Normal map / Specular</td></tr></tbody></table>
{% endtab %}

{% tab title="✒ Example" %}
<figure><img src="../../.gitbook/assets/obraz (22).png" alt=""><figcaption><p>Example of vehicle_tire from vigero.yft</p></figcaption></figure>
{% endtab %}
{% endtabs %}

***

`vehicle_tire_emissive`

{% tabs %}
{% tab title="📚 Description" %}
vehicle\_tire shader with emissive support
{% endtab %}

{% tab title="🎨 Texture Sampler(s)" %}
* [x] Diffuse
* [x] Dirt
* [x] Normal map
* [x] Specular
{% endtab %}

{% tab title="🗺 UV Maps" %}
<table><thead><tr><th width="321">UV Maps</th><th width="379">Texture</th></tr></thead><tbody><tr><td>UVMap 0</td><td>Diffuse /  Dirt / Normal map / Specular</td></tr></tbody></table>
{% endtab %}

{% tab title="✒ Example" %}
<figure><img src="../../.gitbook/assets/tire_emissive.png" alt=""><figcaption><p>Example of vehicle_tire_emissive from tezeractyft</p></figcaption></figure>
{% endtab %}
{% endtabs %}

***

### Vehicle Emissive shaders

`vehicle_dash_emissive`

{% tabs %}
{% tab title="📚 Description" %}
Shader dedicated for emissive dials being lit up at night.
{% endtab %}

{% tab title="🎨 Texture Sampler(s)" %}
* [x] Diffuse
* [x] Specular
{% endtab %}

{% tab title="🗺 UV Maps" %}
<table><thead><tr><th width="320">UV Maps</th><th width="379">Texture</th></tr></thead><tbody><tr><td>UVMap 0</td><td>Diffuse  / Specular</td></tr></tbody></table>
{% endtab %}

{% tab title="✒ Example" %}
<figure><img src="../../.gitbook/assets/obraz (23).png" alt=""><figcaption><p>Example of vehicle_dash_emissive from vigero.yft</p></figcaption></figure>
{% endtab %}
{% endtabs %}

***

`vehicle_dash_emissive_opaque`

{% tabs %}
{% tab title="📚 Description" %}
Shader dedicated for emissive dials being lit up at night for opaque textures.
{% endtab %}

{% tab title="🎨 Texture Sampler(s)" %}
* [x] Diffuse
* [x] Specular
{% endtab %}

{% tab title="🗺 UV Maps" %}
<table><thead><tr><th width="320">UV Maps</th><th width="379">Texture</th></tr></thead><tbody><tr><td>UVMap 0</td><td>Diffuse  / Specular</td></tr></tbody></table>
{% endtab %}

{% tab title="✒ Example" %}
<figure><img src="../../.gitbook/assets/obraz (24).png" alt=""><figcaption><p>Example of converted material for vehicle_dash_emissive_opaque</p></figcaption></figure>
{% endtab %}
{% endtabs %}

***

### Vehicle License plate shaders

`vehicle_licenseplate`

{% tabs %}
{% tab title="📚 Description" %}
Shader responsible for rendering vehicle license plates with changeable text.
{% endtab %}

{% tab title="🎨 Texture Sampler(s)" %}
* [x] Plate background
* [x] Plate background normal map
* [x] Font texture
* [x] Font texture normal map
* [x] Dirt
{% endtab %}

{% tab title="🗺 UV Maps" %}
<table><thead><tr><th width="316">UV Maps</th><th width="379">Texture</th></tr></thead><tbody><tr><td>UVMap 0</td><td>Plate background, Place background bump, Font, Font bump</td></tr><tr><td>UVMap 1</td><td>Dirt</td></tr></tbody></table>
{% endtab %}

{% tab title="✒ Example" %}
<figure><img src="../../.gitbook/assets/obraz (13).png" alt=""><figcaption><p>Example of vehicle_licenseplate from asea2.yft</p></figcaption></figure>
{% endtab %}
{% endtabs %}

***

### Vehicle Miscellaneous shaders

`vehicle_badges`

{% tabs %}
{% tab title="📚 Description" %}
Shader for vehicle badges.
{% endtab %}

{% tab title="🎨 Texture Sampler(s)" %}
* [x] Diffuse
* [x] Normal map
* [x] Specular
{% endtab %}

{% tab title="🗺 UV Maps" %}
<table><thead><tr><th width="321">UV Maps</th><th width="379">Texture</th></tr></thead><tbody><tr><td>UVMap 0</td><td>Diffuse  / Normal map / Specular</td></tr></tbody></table>
{% endtab %}

{% tab title="✒ Example" %}
<figure><img src="../../.gitbook/assets/obraz (10).png" alt=""><figcaption><p>Example of vehicle_badges from asea2.yft</p></figcaption></figure>
{% endtab %}
{% endtabs %}

***

`vehicle_decal`

{% tabs %}
{% tab title="📚 Description" %}
Shader created for adding additional decals, scratches on the vehicle.
{% endtab %}

{% tab title="🎨 Texture Sampler(s)" %}
* [x] Diffuse
* [x] Specular
{% endtab %}

{% tab title="🗺 UV Maps" %}
<table><thead><tr><th width="320">UV Maps</th><th width="379">Texture</th></tr></thead><tbody><tr><td>UVMap 0</td><td>Diffuse  / Specular</td></tr></tbody></table>
{% endtab %}

{% tab title="✒ Example" %}
<figure><img src="../../.gitbook/assets/obraz (14).png" alt=""><figcaption><p>Example of vehicle_decal from ambulance.yft</p></figcaption></figure>
{% endtab %}
{% endtabs %}

***

`vehicle_decal2`

{% tabs %}
{% tab title="📚 Description" %}
Derivated from vehicle\_decal, with dirt support.
{% endtab %}

{% tab title="🎨 Texture Sampler(s)" %}
* [x] Diffuse
* [x] Dirt
* [x] Specular
{% endtab %}

{% tab title="🗺 UV Maps" %}
<table><thead><tr><th width="317">UV Maps</th><th width="379">Texture</th></tr></thead><tbody><tr><td>UVMap 0</td><td>Diffuse  / Dirt / Specular</td></tr></tbody></table>
{% endtab %}

{% tab title="✒ Example" %}
<figure><img src="../../.gitbook/assets/obraz (17).png" alt=""><figcaption><p>Example of vehicle_decal2 from burrito3.yft</p></figcaption></figure>
{% endtab %}
{% endtabs %}

***

`vehicle_detail2`

{% tabs %}
{% tab title="📚 Description" %}
Used to add a leather detail effect to seats and dashboards.
{% endtab %}

{% tab title="🎨 Texture Sampler(s)" %}
* [x] Diffuse
* [x] Normal map
* [x] Specular
{% endtab %}

{% tab title="🗺 UV Maps" %}
<table><thead><tr><th width="369">UV Maps</th><th width="379">Texture</th></tr></thead><tbody><tr><td>UVMap 0</td><td>Diffuse  / Normal map / Specular</td></tr><tr><td>UVMap 1</td><td>Detail (tileable)</td></tr></tbody></table>
{% endtab %}

{% tab title="✒ Example" %}
<figure><img src="../../.gitbook/assets/obraz (16).png" alt=""><figcaption><p>Example of vehicle_detail2 from burrito3.yft</p></figcaption></figure>
{% endtab %}
{% endtabs %}

***

`vehicle_shuts`

{% tabs %}
{% tab title="📚 Description" %}
Shader utilized for inner sides of engine bay, doors, bonnet and boot.
{% endtab %}

{% tab title="🎨 Texture Sampler(s)" %}
* [x] Diffuse
* [x] Normal map
* [x] Specular
{% endtab %}

{% tab title="🗺 UV Maps" %}
<table><thead><tr><th width="320">UV Maps</th><th width="379">Texture</th></tr></thead><tbody><tr><td>UVMap 0</td><td>Diffuse  / Normal map / Specular</td></tr></tbody></table>
{% endtab %}

{% tab title="✒ Example" %}
<figure><img src="../../.gitbook/assets/shuts.png" alt=""><figcaption><p>Example of vehicle_shuts from sentinel2.yft</p></figcaption></figure>
{% endtab %}
{% endtabs %}

***

`vehicle_track/vehicle_track2`

{% tabs %}
{% tab title="📚 Description" %}
Shader for UV animation, **hardcoded usage**, in modded vehicles works only on the left side.
{% endtab %}

{% tab title="🎨 Texture Sampler(s)" %}
* [x] Diffuse
* [x] Normal map
* [x] Specular
{% endtab %}

{% tab title="🗺 UV Maps" %}
<table><thead><tr><th width="320">UV Maps</th><th width="379">Texture</th></tr></thead><tbody><tr><td>UVMap 0</td><td>Diffuse  / Normal map / Specular</td></tr><tr><td>UVMap 1</td><td>Dirt</td></tr></tbody></table>
{% endtab %}

{% tab title="✒ Example" %}
<figure><img src="../../.gitbook/assets/track.png" alt=""><figcaption><p>Example of vehicle_track from manchez2.yft</p></figcaption></figure>
{% endtab %}
{% endtabs %}
