# Grass Batches

Grass batches are represented as a mesh with only vertices, where each vertex represents a grass instance. Attributes are used to store per-grass instance settings.

Geometry nodes are used to generate and preview grass batches. Each grass batch is configured through a list of "templates", which define the models that can appear and their per-model settings (e.g. scale, LOD distance). The geometry nodes modifier then uses these templates to scatter the grass instances over a base mesh.

{% embed url="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FcRAM9lBHCqq3QodZ420I%2Fuploads%2FX8annCOURmw1WgrwQCd6%2Fdemo_grass_batch_gen.mp4?alt=media&token=f2571568-fd53-4c91-aeb6-9a53b1a8de1d" %}

The geometry nodes require Blender 5.0 or newer. Import/export still works on all supported versions, since the grass batch itself is just a regular mesh containing only vertices. This also means some manual editing is possible.

<figure><img src="../../.gitbook/assets/image (113).png" alt="" width="563"><figcaption><p>GrassBatchGen geometry nodes modifier</p></figcaption></figure>

