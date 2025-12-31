# Component:PBS TriplanarMetallic

> Source: https://wiki.resonite.com/Component:PBS_TriplanarMetallic

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:PBS_TriplanarMetallic&diff=106126) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/3/36/PBS_TriplanarMetallicComponent.png/510px-PBS_TriplanarMetallicComponent.png)](https://wiki.resonite.com/File:PBS_TriplanarMetallicComponent.png) **PBS Triplanar Metallic** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

A triplanar shader generates UVs and samples a texture by projecting in world space. The input texture is sampled 3 times, once in each of the world x, y and z axes, and the resulting information is planar projected onto the model, blended by the normal.

They are particularly useful for projecting a texture onto a cubical object without causing stretching of the texture.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `HighPriorityIntegration` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | If true, integrating this asset (e.g. processing procedural assets) gets higher priority than assets with this flag off. An example is user laser procedural meshes. |
| `TextureScale` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | How much to scale up or down the different texture maps. |
| `TextureOffset` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | How much to shift around the position of the different texture maps. |
| `AlbedoColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color to multiply the texture of the albedo (base color) with. Basically a tint. Default white. |
| `AlbedoTexture` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | The texture to use as the color of the surface. |
| `EmissiveColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color to multiply the texture of the emission (glowly color) with. Basically a tint. Default white. |
| `EmissiveMap` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | The texture to use as the glowing (emission) color of the surface. |
| `NormalMap` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | The normal map is used as a way to change the appearance of a surface when shined on by lights, to give the illusion of a raised surface. |
| `NormalScale` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to scale up the effect of the normal map. |
| `OcclusionMap` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | Used to specify surface parts in eternal shadow due to being close to other mesh parts. |
| `TriplanarBlendPower` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How sharp the transition is between different directions of the triplanar texture on the material. |
| `ObjectSpace` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the effects of this material happen in global or local space. Object space is local space (the transform space of the mesh this is on) |
| `OffsetFactor` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much this material should be pushed forwards or backwards on the depth buffer, based on the polygon's slope relative to the camera (i.e. polygons parallel to the camera will not be affected by this).[\[1\]](https://wiki.resonite.com/Component:PBS_TriplanarMetallic#cite_note-Material_OffsetFactor/Units_Desc-1) |
| `OffsetUnits` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much this material should be pushed forwards or backwards on the depth buffer (regardless of the polygon's slope relative to the camera), in units equal to the smallest possible difference for the rendering device being used.[\[1\]](https://wiki.resonite.com/Component:PBS_TriplanarMetallic#cite_note-Material_OffsetFactor/Units_Desc-1) |
| `Culling` | **[Culling](https://wiki.resonite.com/Type:Culling "Type:Culling")** | Whether to show the material on the front, back, or both sides |
| `Transparent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this should render transparent |
| `RenderQueue` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | changes at which point a material renders on the render stack |
| `Metallic` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The metallicness of the material in the absence of the metallic+reflectiveness image map. |
| `Smoothness` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The Smoothness value in the absence of the Metallic+Smoothness image map. |
| `MetallicMap` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | [Metallic Maps](https://wiki.resonite.com/Component:PBS_Metallic#Metallic_Maps "Component:PBS Metallic") |
| `_regular` | **[Shader](https://wiki.resonite.com/Type:Shader "Type:Shader")** | Internal. |
| `_transparent` | **[Shader](https://wiki.resonite.com/Type:Shader "Type:Shader")** | Shader, Internal. |

Fields
Collapse

## Usage

## Examples

## See Also

1. ↑ [Jump up to: 1.0](https://wiki.resonite.com/Component:PBS_TriplanarMetallic#cite_ref-Material_OffsetFactor/Units_Desc_1-0)[1.1](https://wiki.resonite.com/Component:PBS_TriplanarMetallic#cite_ref-Material_OffsetFactor/Units_Desc_1-1)[https://docs.unity3d.com/6000.2/Documentation/Manual/SL-Offset.html](https://docs.unity3d.com/6000.2/Documentation/Manual/SL-Offset.html)

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:PBS\_TriplanarMetallic&oldid=106126](https://wiki.resonite.com/index.php?title=Component:PBS_TriplanarMetallic&oldid=106126)"

Contents