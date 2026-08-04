# LOD Lights

LOD lights are represented as a mesh with only vertices, where each vertex represents a light. Attributes are used to store per-light settings.

"Bake LOD Lights" operator collects the lights of all entities in the map group and generates the `lodlights`/`distlodlights` YMAPs automatically, categorized by size, partitioned, and with streaming extents already computed.

<figure><img src="../../.gitbook/assets/lod_lights_bake.png" alt="" width="563"><figcaption></figcaption></figure>
