# Partitioning

Instead of assigning every map item to a container by hand, a container can be set to **Auto partitioning mode**. Sollumz then splits the items assigned to it into auto-generated child containers, following the same conventions as the vanilla game maps:

* entities and car generators (_strm_),
* entities with large LOD distances (_long_),
* entities marked as critical (_critical_),
* interiors (_milo_),
* and grass.

Large sets are further split into numbered chunks by position.

LOD entities stay in the Auto container itself, which acts as the LOD parent YMAP.

Partitions are regenerated with the Generate Partitions button, or automatically on export if new items were added since.
