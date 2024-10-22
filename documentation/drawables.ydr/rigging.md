# Rigging

Drawables can be rigged using either vertex groups (skinning) or Child Of constraints. The top-level Drawable object must be an armature.

### Skinning

Skinning Drawables works the same way you would normally do it in Blender. Simply create vertex groups where each group's name corresponds to a bone in the armature. Then, add an armature modifier and specify the Drawable as the armature object.

<div align="center">

<figure><img src="../../.gitbook/assets/blender_3Zw5StTfDu.png" alt="" width="503"><figcaption><p>Drawable Model setup for skinning</p></figcaption></figure>

</div>

### Linking bones to Drawable Models

Many Drawables aren't rigged using weighted vertex groups. You can instead link an entire Drawable Model to a bone by using a _Copy Transforms_ constraint.

<figure><img src="../../.gitbook/assets/image (106).png" alt=""><figcaption><p>Sollumz Tools > Drawables > Bone Tools</p></figcaption></figure>

Use the "Add Bone Constraint" operator with the Drawable Model Selected to add a _Copy Transforms_ constraint with the properties setup for correct previewing.

<figure><img src="../../.gitbook/assets/image (105).png" alt=""><figcaption><p>Example <em>Copy Transforms</em> constraint for a Drawable Model</p></figcaption></figure>

{% hint style="info" %}
By default, Blender sets the owner space and target space of the _Copy Transforms_ constraint to "World". This can cause issues when objects are parented to both bones and other objects. Because of this, **make sure to always use the Add Bone Constraint tool when creating **_**Copy Transforms**_** constraints.**
{% endhint %}
