# Component:PBS IntersectSpecular

> Source: https://wiki.resonite.com/Component:PBS_IntersectSpecular

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:PBS_IntersectSpecular&diff=105926) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/3/3b/PBS_IntersectSpecularComponent.png/510px-PBS_IntersectSpecularComponent.png)](https://wiki.resonite.com/File:PBS_IntersectSpecularComponent.png) **PBS Intersect Specular** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

A PBS Intersect Shader (both metallic & specular variants) renders a glow outline when intersecting with opaque materials (any that write to ZBuffer).

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `HighPriorityIntegration` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | If true, integrating this asset (e.g. processing procedural assets) gets higher priority than assets with this flag off. An example is user laser procedural meshes. |
| `_shader` | **[Shader](https://wiki.resonite.com/Type:Shader "Type:Shader")** | Internal. |
| `BeginTransitionStart` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Where the band of color change when the material intercects with a material starts to fade to the intercect colors where the material intercects with another. |
| `BeginTransitionEnd` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Where the band of color change when the material intercects with a material stops to fading to the intercect colors away from the edge where the material intercects with another and actually reaches 100% intercect. |
| `EndTransitionStart` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Where the band of color change when the material intercects with a material starts to fade to original colors on the outer edge. |
| `EndTransitionEnd` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Where the band of color change when the material intercects with a material stops fading and goes back to original colors at the outer edge. |
| `TextureScale` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | How much to scale up or down the different texture maps. |
| `TextureOffset` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | How much to shift around the position of the different texture maps. |
| `AlbedoColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color to multiply the texture of the albedo (base color) with. Basically a tint. Default white. |
| `IntersectAlbedoColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The base color of the material when it is intercecting with another material. |
| `AlbedoTexture` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | The texture to use as the color of the surface. |
| `EmissiveColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color to multiply the texture of the emission (glowly color) with. Basically a tint. Default white. |
| `IntersectEmissiveColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The emission of the material along the edge when it intercects with another material |
| `EmissiveMap` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | The texture to use as the glowing (emission) color of the surface. |
| `NormalMap` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | The normal map is used as a way to change the appearance of a surface when shined on by lights, to give the illusion of a raised surface. |
| `NormalScale` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to scale up the effect of the normal map. |
| `OcclusionMap` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | Used to specify surface parts in eternal shadow due to being close to other mesh parts. |
| `Culling` | **[Culling](https://wiki.resonite.com/Type:Culling "Type:Culling")** | Whether to show the material on the front, back, or both sides |
| `OffsetFactor` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much this material should be pushed forwards or backwards on the depth buffer, based on the polygon's slope relative to the camera (i.e. polygons parallel to the camera will not be affected by this).[\[1\]](https://wiki.resonite.com/Component:PBS_IntersectSpecular#cite_note-Material_OffsetFactor/Units_Desc-1) |
| `OffsetUnits` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much this material should be pushed forwards or backwards on the depth buffer (regardless of the polygon's slope relative to the camera), in units equal to the smallest possible difference for the rendering device being used.[\[1\]](https://wiki.resonite.com/Component:PBS_IntersectSpecular#cite_note-Material_OffsetFactor/Units_Desc-1) |
| `RenderQueue` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | changes at which point a material renders on the render stack |
| `SpecularColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | Specular Tint. Behaves like PBS Specular Tinting |
| `SpecularMap` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | [Specular Maps](https://wiki.resonite.com/Component:PBS_Specular#Specular_Maps "Component:PBS Specular") |

Fields
Collapse

## Usage

## Examples

## See Also

1. ↑ [Jump up to: 1.0](https://wiki.resonite.com/Component:PBS_IntersectSpecular#cite_ref-Material_OffsetFactor/Units_Desc_1-0)[1.1](https://wiki.resonite.com/Component:PBS_IntersectSpecular#cite_ref-Material_OffsetFactor/Units_Desc_1-1)[https://docs.unity3d.com/6000.2/Documentation/Manual/SL-Offset.html](https://docs.unity3d.com/6000.2/Documentation/Manual/SL-Offset.html)

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:PBS\_IntersectSpecular&oldid=105926](https://wiki.resonite.com/index.php?title=Component:PBS_IntersectSpecular&oldid=105926)"

Contents