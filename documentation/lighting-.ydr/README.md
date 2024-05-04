---
description: >-
  Lights are well, lights that are embedded into .ydr or .yft objects. there is
  many different settings for these lights which can make it very tricky and
  confusing to get right.
---

# 💡 Lighting (.ydr)

## Before we begin

Some things to keep in mind before we start:

* Your best references are vanilla lights (Rockstar knows best)
* Trial and error is key

## Difference between light types

There is 3 different types of lights, Point, Spot and capsule.

knowing when and why to use which type of light is a key skill in achieving good lighting.

<figure><img src="../../.gitbook/assets/image (90).png" alt=""><figcaption><p>Point Light</p></figcaption></figure>

A point light is exactly what it sounds like. a point that emits light in a radius around it.

<figure><img src="../../.gitbook/assets/image (91).png" alt=""><figcaption><p>Spot Light</p></figcaption></figure>

A Spot light is essentially just a cone that starts at one point and gradually widens towards the other end.

## Light Parameters

Lights have many different settings and parameters, some more important than others.

First we will be covering the General properties that are essential to all lights.

<figure><img src="../../.gitbook/assets/image (92).png" alt=""><figcaption></figcaption></figure>

First you have the color setting, not much needs to be said about this.

next is the Insensity setting, this defines the strength or how bright the light will shine.

after that is the Falloff Exponent, you can think of this one as the radius of the light and the higher the value, the larger the light will be.

Shadow Clip Start can basically be ignored, its not very important.

### Spot Specific Settings

<figure><img src="../../.gitbook/assets/image (93).png" alt=""><figcaption></figcaption></figure>

The Cone Outer Angle value defines the overall size and width of the spot light.

Cone Inner Angle defines the falloff or gradient you could say or "blend" between the inner and outer cone.

### Misc Properties

These are parameters that dont fall into any other categeory.

<figure><img src="../../.gitbook/assets/image (94).png" alt=""><figcaption></figcaption></figure>

Currently, it is unknown what Light Hash or Group ID does, but Light Hash is commonly used for rockstars lights.

Projected Texture hash is just the name of a texture if you want the light to project it.

Flashiness defines how and if the light should flicker or flash.

### Volume Properties

<figure><img src="../../.gitbook/assets/image (95).png" alt=""><figcaption></figcaption></figure>

These settings are for if you have the Enable Volume light flag enabled.

Volume Size Scale obviously sets the size of the volumetric lighting.

Volume Outer Color sets the outside colour of the volumetric light.

Volume Outer Intensity sets how vibrant or bright the outer colour should be.

Volume Outer Exponent is used as sort of a blending between the inner and outer volume colours.

### Distance Properties

These parameters define the distance at which certain things about the light fade.

<figure><img src="../../.gitbook/assets/image (96).png" alt=""><figcaption></figcaption></figure>

### Culling Plane Properties

<figure><img src="../../.gitbook/assets/image (97).png" alt=""><figcaption></figcaption></figure>

The culling plane is used to define where the light should be blocked from shining, mainly used to stop light from passing through walls.

### Corona Properties

<figure><img src="../../.gitbook/assets/image (98).png" alt=""><figcaption></figcaption></figure>

These settings effect the glowing center of the light (Corona)

Size obviously effects the size of it.

Corona Intensity defines how noticable or bright it should be

It is unsure what Corona Z Bias does exactly.



### Advanced Properties

<figure><img src="../../.gitbook/assets/image (99).png" alt=""><figcaption></figcaption></figure>

Effects how blurry the shadows are casted from the light.
