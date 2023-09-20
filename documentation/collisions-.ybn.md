# 💥 Collisions (.ybn)

Collisions are well, collisions. whether that is for players, bullets, vehicles etc.\
There is 3 main types of .ybns, the normal version(s), hi@ versions which is for weapon bullets, and ma@ collisions that are used to procedurally spawn grass and other things like garbage on the street.

```
BoundComposite
     BoundGeometryBVH
          BoundPolyMesh
          BoundBox
          BoundPolyBox
```

{% hint style="info" %}
A very common mistake users make is not applying a Flag Preset to the Bound GeometryBVH, resulting in the collision not working in game.
{% endhint %}

The Bound Composite is the top most part of the hierarchy, it doesnt control much on its own.\
\
The Bound GeometryBVH controls things like which things collide with the Bound Poly Mesh / Boxes.\
&#x20;![](<../.gitbook/assets/image (66).png>)\
You can disable or enable certain flags here t o disable collision for specific object types.\
\
The Bound Poly Mesh / Box is the collision model itself, what you are actually colliding with.\
It is here where you can add or remove Collision materials and apply flags to said materials to control the physics of the collisions further.\
![](<../.gitbook/assets/image (67).png>)\
\
Also, the "Procedural ID" setting is used mainly for ma@ collision ybns to spawn procedural objects like trash on the ground.\
The "Room ID" Setting is used for setting up different rooms for MLOs.\
