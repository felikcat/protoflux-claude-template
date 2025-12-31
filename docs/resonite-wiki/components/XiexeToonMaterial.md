# Component:XiexeToonMaterial

> Source: https://wiki.resonite.com/Component:XiexeToonMaterial

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:XiexeToonMaterial&diff=113627) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/d/de/XiexeToonMaterialComponent.png/510px-XiexeToonMaterialComponent.png)](https://wiki.resonite.com/File:XiexeToonMaterialComponent.png) **Xiexe Toon Material** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **XiexeToonMaterial** component was originally made to be a toon material Component, but is widely considered a robust material. It can recreate most effects of the poiyomi toon material when combined with drives, material stacking, and [manual packing of texture channels](https://wiki.resonite.com/Channel_packing "Channel packing") to make the textures compatible.

Decals are also possible via stacking [PBS\_Metallic](https://wiki.resonite.com/Component:PBS_Metallic "Component:PBS Metallic") layers using extra meshes, then setting them to cutout or alpha with an image set to clamp. The values do not transfer 1:1

TODO: Equation to convert poiyomi decal stuff to Resonite

A Japanese guide with visual examples for using the XiexeToon created by akiRAM can be found at the following link: [https://note.com/akiram\_vr/n/n5e55290e2cee](https://note.com/akiram_vr/n/n5e55290e2cee)

It was written for the predecessor to Resonite, however as stated on the page most settings are very similar so is still very relevant.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `HighPriorityIntegration` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | If true, integrating this asset (e.g. processing procedural assets) gets higher priority than assets with this flag off. An example is user laser procedural meshes. |
| `MainTexture` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | The main color map of the material. |
| `Color` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The surface color texture of the material. |
| `UseVertexColors` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the material should use vertex colors from the mesh. |
| `VertexColorInterpolationSpace` | **[ColorProfile](https://wiki.resonite.com/Type:ColorProfile "Type:ColorProfile")** | How to interpolate vertex colors on the mesh. |
| `BlendMode` | **[BlendMode](https://wiki.resonite.com/Type:BlendMode "Type:BlendMode")** | How to blend this material's colors vs what it rendered on top of. |
| `ZWrite` | **[ZWrite](https://wiki.resonite.com/Type:ZWrite "Type:ZWrite")** | whether this material should respect the distance it is from the camera. |
| `AlphaClip` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Any alpha value below this amount is not rendered for any given pixel when cutout is enabled. |
| `MainTextureScale` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The UV scaling of the main texture. |
| `MainTextureOffset` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The UV offset of the main texture. |
| `Saturation` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The saturation multiplier of `MainTexture`. |
| `NormalMap` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | The normal map is used as a way to change the appearance of a surface when shined on by lights, to give the illusion of a raised surface. |
| `NormalMapScale` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The UV scaling of the normal map texture. |
| `NormalMapOffset` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The UV offset of the normal texture. |
| `NormalScale` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to scale up the effect of the normal map. |
| `Metallic` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The metallicness of the material in the absence of the metallic+reflectiveness image map. |
| `Glossiness` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The glossiness of the material in the absence of `MetallicGlossMap`. |
| `Reflectivity` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The reflectivity of the material in the absence of `MetallicGlossMap`. |
| `MetallicGlossMap` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | A packed channel texture for Metallic, glossyness, and reflectivity. |
| `MetallicGlossMapScale` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The UV scaling of the `MetallicGlossMap`. |
| `MetallicGlossMapOffset` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The UV offset of the `MetallicGlossMap`. |
| `EmissionMap` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | The glow or emission color map. |
| `EmissionColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The tint of the emission color. |
| `EmissionMapScale` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The UV scaling of the emission texture. |
| `EmissionMapOffset` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The UV offset of the emission texture. |
| `RimColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | Rim Lighting Color |
| `RimAlbedoTint` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much the rim lighting effects albedo tint. |
| `RimAttenuationEffect` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The strength of the rim light |
| `RimIntensity` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Brightness of rim lighting |
| `RimRange` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Size of light area of the shadowramp |
| `RimThreshold` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Size of rim light area |
| `RimSharpness` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Definition of the shadowramp |
| `SpecularIntensity` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Unused. |
| `SpecularArea` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Unused. |
| `Matcap` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | A texture that looks like a sphere with reflection shading on it. Used to make the fake reflection map. |
| `MatcapTint` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color tint to apply to `Matcap`. |
| `OcclusionMap` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | Used to specify surface parts in eternal shadow due to being close to other mesh parts. |
| `OcclusionMapScale` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The UV scale of `OcclusionMap` |
| `OcclusionMapOffset` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The UV offset of `OcclusionMap`. |
| `OcclusionColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color of the occlusion effect. |
| `Outline` | **[OutlineStyle](https://wiki.resonite.com/Component:XiexeToonMaterial#OutlineStyle)** | The outline style to use. |
| `OutlineWidth` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The thickness of the outline around the mesh. |
| `OutlineColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color of the outline around the mesh. |
| `OutlineAlbedoTint` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the outline is tinted by albedo. |
| `OutlineMask` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | Grayscale mask that determines relative thickeness of outline. Black is no outline. White is 100% of the OutlineWidth value. |
| `ShadowRamp` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | The shadow ramp used to influence what shadows look like on a model. |
| `ShadowRampMask` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | Grayscale mask that selects which pixel row of the Shadow Ramp texture to use for a given texel. |
| `ShadowRampMaskScale` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The UV scale of `ShadowRampMask`. |
| `ShadowRampMaskOffset` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The UV offset of `ShadowRampMask`. |
| `ShadowRim` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | Color of the dark rim light |
| `ShadowSharpness` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Definition of all shadows applied to the material |
| `ShadowRimRange` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Size of the dark section of the shadowramp |
| `ShadowRimThreshold` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Size of the dark section of the shadowramp |
| `ShadowRimSharpness` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Definition of the dark section of the shadowramp |
| `ShadowRimAlbedoTint` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much the albedo color influences the dark section of the shadowramp |
| `ThicknessMap` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | The thickness map of the surface. Used to make subsurface effects. |
| `ThicknessMapScale` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The UV scale of `ThicknessMap`. |
| `ThicknessMapOffset` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The UV offset of `ThicknessMap` |
| `SubsurfaceColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color of the subsurface effect. |
| `SubsurfaceDistortion` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Strength of subsurface color |
| `SubsurfacePower` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Strength of subsurface color |
| `SubsurfaceScale` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Strength of subsurface color |
| `OffsetFactor` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much this material should be pushed forwards or backwards on the depth buffer, based on the polygon's slope relative to the camera (i.e. polygons parallel to the camera will not be affected by this).[\[1\]](https://wiki.resonite.com/Component:XiexeToonMaterial#cite_note-Material_OffsetFactor/Units_Desc-1) |
| `OffsetUnits` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much this material should be pushed forwards or backwards on the depth buffer (regardless of the polygon's slope relative to the camera), in units equal to the smallest possible difference for the rendering device being used.[\[1\]](https://wiki.resonite.com/Component:XiexeToonMaterial#cite_note-Material_OffsetFactor/Units_Desc-1) |
| `Culling` | **[Culling](https://wiki.resonite.com/Type:Culling "Type:Culling")** | Whether to show the material on the front, back, or both sides |
| `ColorMask` | **[ColorMask](https://wiki.resonite.com/Type:ColorMask "Type:ColorMask")** | What colors behind the material should make it through the filter. |
| `AlbedoUV` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The UV map index Albedo map should use. |
| `NormalUV` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The UV map index normal map should use. |
| `MetallicUV` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The UV map index metallic map should use. |
| `ThicknessUV` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The UV map index Thickness map should use. |
| `OcclusionUV` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The UV map index occlusion map should use. |
| `EmissionUV` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The UV map index emission map should use. |
| `RenderQueue` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | changes at which point a material renders on the render stack |
| `__legacyCutout` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Internal. |
| `_regular` | **[Shader](https://wiki.resonite.com/Type:Shader "Type:Shader")** | Internal. |
| `_outline` | **[Shader](https://wiki.resonite.com/Type:Shader "Type:Shader")** | Internal. |

Fields
Collapse

## Usage

## OutlineStyle

|     |     |
| --- | --- |
| **Name:** | OutlineStyle |
| **Type:** | `FrooxEngine.XiexeToonMaterial+OutlineStyle` |

[Nested Enum](https://wiki.resonite.com/Category:Components_With_Nested_Enums "Category:Components With Nested Enums")

Defines the type of outline to show on the material.

| Name | Value | Description |
| --- | --- | --- |
| `None` | 0 | There will be no outline. |
| `Lit` | 1 | The outline will be lit. |
| `Emissive` | 2 | The outline will be emissive. |

Values

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

For those who use Substance Painter, the following presets are also available:

[https://github.com/PointerOffset/Xiexie-Substance-Resonite-Templates](https://github.com/PointerOffset/Xiexie-Substance-Resonite-Templates)

[https://github.com/Epimonster/resonite-substance-support](https://github.com/Epimonster/resonite-substance-support)

1. ↑ [Jump up to: 1.0](https://wiki.resonite.com/Component:XiexeToonMaterial#cite_ref-Material_OffsetFactor/Units_Desc_1-0)[1.1](https://wiki.resonite.com/Component:XiexeToonMaterial#cite_ref-Material_OffsetFactor/Units_Desc_1-1)[https://docs.unity3d.com/6000.2/Documentation/Manual/SL-Offset.html](https://docs.unity3d.com/6000.2/Documentation/Manual/SL-Offset.html)

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:XiexeToonMaterial&oldid=113627](https://wiki.resonite.com/index.php?title=Component:XiexeToonMaterial&oldid=113627)"

Contents