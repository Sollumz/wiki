---
description: >-
  Used to add things like particles, ped spawns, ladders, and light shafts to be
  attached to the entity
---

# Archetype Extensions

<figure><img src="../../.gitbook/assets/image (57).png" alt="" width="389"><figcaption></figcaption></figure>

### CExtensionDefExpression

Used for:\


<figure><img src="../../.gitbook/assets/image (58).png" alt="" width="381"><figcaption></figcaption></figure>

| Setting                    | Description                                |
| -------------------------- | ------------------------------------------ |
| Name                       |                                            |
| Expression Dictionary Name |                                            |
| Expression Name            |                                            |
| Creature Metadata Name     |                                            |
| Initialize on Collision    |                                            |
| Offset Position XYZ        | Extension offset relative to entity origin |

### CExtensionProcObject

Used For: Attaching / Spreading procedural objects\


<figure><img src="../../.gitbook/assets/image (59).png" alt="" width="383"><figcaption></figcaption></figure>

<table><thead><tr><th width="222">Setting</th><th>Description</th></tr></thead><tbody><tr><td>Name</td><td>Extension Name</td></tr><tr><td>Radius Inner</td><td>Inside radius of a circle around the extension</td></tr><tr><td>Radius Outer</td><td>outside radius of a circle around the extension</td></tr><tr><td>Spacing</td><td>Distance between procedural objects</td></tr><tr><td>Min Scale</td><td>Lowest possible scale value</td></tr><tr><td>Max Scale</td><td>Highest possible scale value</td></tr><tr><td>Min Scale Z</td><td>Lowest possible scale value on the Z axis</td></tr><tr><td>Max Scale Z</td><td>Highest possible scale value on the Z axis</td></tr><tr><td>Min Z Offset</td><td>lowest possible offset on the Z Axis</td></tr><tr><td>Max Z Offset</td><td>Highest possible offset on the Z Axis</td></tr><tr><td>Object Hash</td><td>procedural object to use</td></tr><tr><td>Flags</td><td></td></tr><tr><td>Offset Position XYZ</td><td>Extension offset relative to entity origin</td></tr></tbody></table>

### CExtensionDefWindDisturbance

Used for:\


<figure><img src="../../.gitbook/assets/image (60).png" alt="" width="381"><figcaption></figcaption></figure>

| Setting             | Description                                |
| ------------------- | ------------------------------------------ |
| Name                | Extension Name                             |
| Offset Rotation XYZ | Extension rotation                         |
| Disturbance Type    |                                            |
| Bone Tag            | Linked bone's Bone Tag(Optional?)          |
| Size XYZW           |                                            |
| Flags               |                                            |
| Offset Position XYZ | Extension offset relative to entity origin |

### CExtensionDefSpawnPointOverride

Used For: Spawning / overriding ped spawns\


<figure><img src="../../.gitbook/assets/image (61).png" alt="" width="383"><figcaption></figcaption></figure>

| Setting              | Description                                |
| -------------------- | ------------------------------------------ |
| Name                 | Extension Name                             |
| Scenario Type        | Scenario type from .ymt scenarios          |
| iTime Start Override | When the override should start             |
| iTime End Override   | When the override should end               |
| Group                | Ped Group                                  |
| Model Set            | Ped Model Set                              |
| Radius               | Radius of the Spawn Point Override         |
| Time Till ped Leaves | Time until ped stops task (in minutes?)    |
| Available in MP/SP   | Whether it is SP only or MP                |
| Scenario Flags       |                                            |
| Offset Position XYZ  | Extension offset relative to entity origin |

### CExtensionDefSpawnPoint

Used For: Attaching peds / ped scenarios to objects\


<figure><img src="../../.gitbook/assets/image (62).png" alt="" width="383"><figcaption></figcaption></figure>

| Setting              | Description                                                           |
| -------------------- | --------------------------------------------------------------------- |
| Name                 | Extension Name                                                        |
| Offset Rotation XYZ  | Extension rotation                                                    |
| Spawn Type           |                                                                       |
| Ped Type             |                                                                       |
| Group                | Ped Group                                                             |
| Interior             | Interior Name (if inside one)                                         |
| Required Map         |                                                                       |
| Probability          | Chance for the scenario to spawn                                      |
| Time Till Ped Leaves | Time until ped stops task (in minutes?)                               |
| Radius               | Radius of the Spawn Point                                             |
| Start                | Time the scenario starts                                              |
| End                  | Time the scenario ends                                                |
| High Priority        | Prioritizes spawning of scenario                                      |
| Extended Range       | Extend range at which the scenario can spawn relative to the player   |
| Short Range          | Decrease range at which the scenario can spawn relative to the player |
| Available in MP/SP   | Whether it is SP only or MP                                           |
| Scenario Flags       |                                                                       |
| Offset Position XYZ  | Extension offset relative to entity origin                            |

### CExtensionDefLightShaft

Used For: Light Rays / God Rays

<figure><img src="../../.gitbook/assets/image (63).png" alt="" width="378"><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (64).png" alt="" width="383"><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (65).png" alt="" width="375"><figcaption></figcaption></figure>

| Setting                | Description                                                      |
| ---------------------- | ---------------------------------------------------------------- |
| Density Type           | How dense the light shaft should be                              |
| Volume Type            | Shape of the shaft                                               |
| Scale By Sun Intensity | Use in game sun intensity to effect brightness                   |
| Direction Amount       |                                                                  |
| Length                 | Length of the Light Shaft                                        |
| Color                  | Color of the Light Shaft                                         |
| Intensity              | Intensity of the Light Shaft                                     |
| Flashiness             | Flags for how fast and if the Light Shaft should flash / flicker |
| Flags                  |                                                                  |
| Fade In Time Start     | When the Light Shaft should begin to appear                      |
| Fade in time End       | when the Light Shaft is fully visible                            |
| Fade Out Time Start    | When the Light Shaft should begin fading away                    |
| Fade Out Time End      | when the Light Shaft Shouldnt be visible                         |
| Fade Distance Start    | Distance at which the Light Shaft begins Fading                  |
| Fade Distance End      | Distance at which the Light Shaft is fully Faded                 |
| Softness               |                                                                  |
|                        |                                                                  |
| Corner A XYZ           | Top Left Corner Coords                                           |
| Corner B XYZ           | Top Right Corner Coords                                          |
| Corner C XYZ           | Bottom Right Corner Coords                                       |
| Corner D XYZ           | Bottom Left Corner Coords                                        |
| Offset Position XYZ    | Extension offset relative to entity origin                       |
