# Occluders

Occluders are used as a rendering optimization to determine which objects are hidden from view and avoid rendering them. These are stored as box occluders (oriented boxes) or model occluders (low-poly triangle meshes).

Occluders are represented as a red semitransparent mesh.

<figure><img src="../../.gitbook/assets/image (116).png" alt=""><figcaption></figcaption></figure>

The list of occluders can be found in Occluders tab panel in the sidebar.

<figure><img src="../../.gitbook/assets/image (114).png" alt="" width="563"><figcaption><p>Occluders tab panel</p></figcaption></figure>

Each occluder can be linked to multiple mesh objects which are merged together on export. Each mesh object can use one of the following export modes:

* **Automatic**: automatically detects box-shaped mesh islands (upright boxes or planes) and exports them as box occluders; everything else as model occluders.
* **Boxes Only**: all mesh islands must be box-shaped. Non-box islands are skipped with a warning.
* **Models Only**: export the mesh as-is as model occluders, without attempting box conversion

<figure><img src="../../.gitbook/assets/image (115).png" alt="" width="181"><figcaption><p>Occluder export modes</p></figcaption></figure>
