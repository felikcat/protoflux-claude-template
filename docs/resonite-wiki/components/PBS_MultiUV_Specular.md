# Component:PBS MultiUV Specular

> Source: https://wiki.resonite.com/Component:PBS_MultiUV_Specular

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:PBS_MultiUV_Specular&diff=105950) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/6/65/PBS_MultiUV_SpecularComponent.png/510px-PBS_MultiUV_SpecularComponent.png)](https://wiki.resonite.com/File:PBS_MultiUV_SpecularComponent.png) **PBS Multi UV Specular** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **PBS\_MultiUV\_Specular** component is used to create a multiple image layered effect (pairs) except for a lack of a second Specular map image.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `HighPriorityIntegration` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | If true, integrating this asset (e.g. processing procedural assets) gets higher priority than assets with this flag off. An example is user laser procedural meshes. |
| `_shader` | **[Shader](https://wiki.resonite.com/Type:Shader "Type:Shader")** | Internal. |
| `AlbedoScale` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | How much to scale up or down the albedo texture maps. |
| `AlbedoOffset` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | How much to push around the position of the albedo texture maps. |
| `AlbedoUV` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The UV map index Albedo map should use. |
| `EmissionMapScale` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The UV scaling of the emission texture. |
| `EmissionMapOffset` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The UV offset of the emission texture. |
| `EmissionMapUV` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | What UV map data index the emission map can use |
| `NormalMapScale` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The UV scaling of the normal map texture. |
| `NormalMapOffset` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The UV offset of the normal texture. |
| `NormalMapUV` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | What UV Map data index on the mesh the normal maps should use. |
| `OcclusionMapScale` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The UV scale of `OcclusionMap` |
| `OcclusionMapOffset` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The UV offset of `OcclusionMap`. |
| `OcclusionMapUV` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | What UV map data index in the mesh data the occlusion maps should use. |
| `SecondaryAlbedoScale` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The amount to scale up or down the UV of the secondary albedo texture map. |
| `SecondaryAlbedoOffset` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | How much to push around or position the UV of the secondary albedo texture. |
| `SecondaryAlbedoUV` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The UV map to use for the secondary albedo texture on this material. |
| `SecondaryEmissionMapScale` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The scaling of the UV maps on the second emissive map for this material. |
| `SecondaryEmissionMapOffset` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The offset or positioning of the UVs for the secondary emission map of this material. |
| `SecondaryEmissionMapUV` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The UV map index to use for mesh UV data for this material's secondary emission map. |
| `AlbedoColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color to multiply the texture of the albedo (base color) with. Basically a tint. Default white. |
| `AlbedoTexture` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | The texture to use as the color of the surface. |
| `EmissiveColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color to multiply the texture of the emission (glowly color) with. Basically a tint. Default white. |
| `EmissiveMap` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | The texture to use as the glowing (emission) color of the surface. |
| `NormalMap` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | The normal map is used as a way to change the appearance of a surface when shined on by lights, to give the illusion of a raised surface. |
| `NormalScale` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to scale up the effect of the normal map. |
| `OcclusionMap` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | Used to specify surface parts in eternal shadow due to being close to other mesh parts. |
| `SecondaryAlbedoTexture` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | The texture image to use for the secondary albedo map for this material. This determines a multiplicative secondary base color texture. |
| `SecondaryEmissiveColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The emissive color tint (multiplicative) for the secondary emission map for this material. |
| `SecondaryEmissiveMap` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | The secondary multiplicative emission map texture for this material. |
| `Culling` | **[Culling](https://wiki.resonite.com/Type:Culling "Type:Culling")** | Whether to show the material on the front, back, or both sides |
| `AlphaHandling` | **[AlphaHandling](https://wiki.resonite.com/Type:AlphaHandling "Type:AlphaHandling")** | How to handle alpha values in pixels on the `AlbedoTexture`. |
| `AlphaClip` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Any alpha value below this amount is not rendered for any given pixel when cutout is enabled. |
| `OffsetFactor` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much this material should be pushed forwards or backwards on the depth buffer, based on the polygon's slope relative to the camera (i.e. polygons parallel to the camera will not be affected by this).[\[1\]](https://wiki.resonite.com/Component:PBS_MultiUV_Specular#cite_note-Material_OffsetFactor/Units_Desc-1) |
| `OffsetUnits` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much this material should be pushed forwards or backwards on the depth buffer (regardless of the polygon's slope relative to the camera), in units equal to the smallest possible difference for the rendering device being used.[\[1\]](https://wiki.resonite.com/Component:PBS_MultiUV_Specular#cite_note-Material_OffsetFactor/Units_Desc-1) |
| `RenderQueue` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | changes at which point a material renders on the render stack |
| `SpecularColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | Specular Tint. Behaves like PBS Specular Tinting |
| `SpecularMap` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | [Specular Maps](https://wiki.resonite.com/Component:PBS_Specular#Specular_Maps "Component:PBS Specular") |
| `SpecularMapScale` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The scaling of the UV map of the Specular map for the material. |
| `SpecularMapOffset` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The offset or positioning of the Specular map on the surface. |
| `SpecularMapUV` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The Specular map image for defining smoothness/Specular on different parts of the material surface. |

Fields
Collapse

## Usage

## Examples

## See Also

1. ↑ [Jump up to: 1.0](https://wiki.resonite.com/Component:PBS_MultiUV_Specular#cite_ref-Material_OffsetFactor/Units_Desc_1-0)[1.1](https://wiki.resonite.com/Component:PBS_MultiUV_Specular#cite_ref-Material_OffsetFactor/Units_Desc_1-1)[https://docs.unity3d.com/6000.2/Documentation/Manual/SL-Offset.html](https://docs.unity3d.com/6000.2/Documentation/Manual/SL-Offset.html)

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:PBS\_MultiUV\_Specular&oldid=105950](https://wiki.resonite.com/index.php?title=Component:PBS_MultiUV_Specular&oldid=105950)"

Contents