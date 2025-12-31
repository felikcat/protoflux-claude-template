# Component:PBS Metallic

> Source: https://wiki.resonite.com/Component:PBS_Metallic

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:PBS_Metallic&diff=114871) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/2/2d/PBS_MetallicComponent.png/510px-PBS_MetallicComponent.png)](https://wiki.resonite.com/File:PBS_MetallicComponent.png) **PBS\_Metallic** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

PBS Metallic is a [physically-based](https://en.wikipedia.org/wiki/Physically_based_rendering) material that uses a Metallic-Smoothness (MS) map to store data about the metallicity and smoothness of an object. It is based on the Unity 5 Standard PBR Setup.

For information about the maps and their properties read on!

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `HighPriorityIntegration` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | If true, integrating this asset (e.g. processing procedural assets) gets higher priority than assets with this flag off. An example is user laser procedural meshes. |
| `_shader` | **[Shader](https://wiki.resonite.com/Type:Shader "Type:Shader")** | Internal. |
| `TextureScale` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | How much to scale up or down the different texture maps. |
| `TextureOffset` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | How much to shift around the position of the different texture maps. |
| `DetailTextureScale` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | How much to scale up or down the different detail texture maps. |
| `DetailTextureOffset` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | How much to shift around the position of the different detail texture maps. |
| `AlbedoColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color to multiply the texture of the albedo (base color) with. Basically a tint. Default white. |
| `AlbedoTexture` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | The texture to use as the color of the surface. |
| `EmissiveColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color to multiply the texture of the emission (glowly color) with. Basically a tint. Default white. |
| `EmissiveMap` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | The texture to use as the glowing (emission) color of the surface. |
| `NormalScale` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to scale up the effect of the normal map. |
| `NormalMap` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | The normal map is used as a way to change the appearance of a surface when shined on by lights, to give the illusion of a raised surface. |
| `HeightMap` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | The height map changes the position that pixels of the surface are rendered so they appear further or closer to the actual surface. Like a parallax effect. Can cause artifacts around edges. |
| `HeightScale` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How strong the height parallax effect should be. |
| `OcclusionMap` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | Used to specify surface parts in eternal shadow due to being close to other mesh parts. |
| `DetailAlbedoTexture` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | A multiplied layer of albedo on top of the default `AlbedoTexture`. |
| `DetailNormalMap` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | A layered normal map on top of the default `NormalMap`. |
| `DetailNormalScale` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to scale up the effect of the detail normal map. |
| `BlendMode` | **[BlendMode](https://wiki.resonite.com/Type:BlendMode "Type:BlendMode")** | How to blend this material's colors vs what it rendered on top of. |
| `AlphaCutoff` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | If `BlendMode` is set to cutout, discard rendering of pixels for the surface that fall below this alpha threshold. |
| `OffsetFactor` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much this material should be pushed forwards or backwards on the depth buffer, based on the polygon's slope relative to the camera (i.e. polygons parallel to the camera will not be affected by this).[\[1\]](https://wiki.resonite.com/Component:PBS_Metallic#cite_note-Material_OffsetFactor/Units_Desc-1) |
| `OffsetUnits` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much this material should be pushed forwards or backwards on the depth buffer (regardless of the polygon's slope relative to the camera), in units equal to the smallest possible difference for the rendering device being used.[\[1\]](https://wiki.resonite.com/Component:PBS_Metallic#cite_note-Material_OffsetFactor/Units_Desc-1) |
| `RenderQueue` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | changes at which point a material renders on the render stack |
| `Metallic` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much metallicness the surface should have if `MetallicMap` is not specified. |
| `Smoothness` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much smoothness the surface should have if `MetallicMap` is not specified. |
| `MetallicMap` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | [Metallic Maps](https://wiki.resonite.com/Component:PBS_Metallic#Metallic_Maps) |

Fields
Collapse

## Usage

### Normal Maps

- Normal maps are encoded with GLNormals

### Metallic Maps

This Material type uses a Metallic Map for determining:

- Metallic Levels
- Ambient Occlusion/Height
- Smoothness

This information is [packed](https://wiki.resonite.com/Channel_packing "Channel packing") into different channels within the Metallic Map using the following pattern:

- **R(Red Channel)**: Metallic

  - The Red Channel determines how metallic a material is.
  - Metals are usually 1 in this channel and non-metals (also known as dielectrics) are 0
  - When choosing Metallic values, do remember that items in the real world aren't perfect. Imperfections and randomness is good! A common misconception is that pixels within a metallic map must be pure 0 or 1 values, however this is not the case. If you were able to zoom in far enough into a material you could observe pure metal and pure non-metal parts (rust would be metal with a separate layer of oxidized material), but with textures, you only have a limited number of pixels to represent individual characteristics of materials. When authoring these textures, what you are actually doing is describing the average characteristic in the area of interest. It is therefore accurate to describe materials such as rust as somewhere between 0 and 1 on average in an area depending on how much oxidation versus metal there is.
- **G (Green Channel)**: Ambient Occlusion/Height

  - This allows you to pack either the Ambient Occlusion or the Height map data into one image and re-use it in those inputs to the material, depending on which you prefer to use.
- **Alpha**: Smoothness

  - High Alpha means High Smoothness
  - Low Alpha is Low Smoothness

Resonite uses the Unity Standard Shader Maps for this Material, for more information please see [this guide](https://docs.unity3d.com/Manual/StandardShaderMaterialCharts.html) for more information.

### Other Maps

**TODO**

Unity declares Green : Occlusion and Height as interchangeable and usable for both slots

[https://forum.unity.com/threads/standard-shader-metallic-texture-packing.314283/](https://forum.unity.com/threads/standard-shader-metallic-texture-packing.314283/)

R: Metalness

G: Occlusion/Height

A: Smoothness

## Examples

## Further Reading

You may be interested in the following other pages:

- [PBS Specular](https://wiki.resonite.com/PBS_Specular "PBS Specular") \- Documentation on Resonite's PBS Specular Material. This is often paired or compared to PBS Metallic.

1. ↑ [Jump up to: 1.0](https://wiki.resonite.com/Component:PBS_Metallic#cite_ref-Material_OffsetFactor/Units_Desc_1-0)[1.1](https://wiki.resonite.com/Component:PBS_Metallic#cite_ref-Material_OffsetFactor/Units_Desc_1-1)[https://docs.unity3d.com/6000.2/Documentation/Manual/SL-Offset.html](https://docs.unity3d.com/6000.2/Documentation/Manual/SL-Offset.html)

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:PBS\_Metallic&oldid=114871](https://wiki.resonite.com/index.php?title=Component:PBS_Metallic&oldid=114871)"

Contents