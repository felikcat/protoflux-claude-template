# Component:PBSLerpSpecular

> Source: https://wiki.resonite.com/Component:PBSLerpSpecular

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:PBSLerpSpecular&diff=105839) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/a/a6/PBSLerpSpecularComponent.png/510px-PBSLerpSpecularComponent.png)](https://wiki.resonite.com/File:PBSLerpSpecularComponent.png) **PBS Lerp Specular** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **PBSLerpSpecular** component also known as Lerping Material, lerp material, fading material, transitioning material, blending material, changing material. Is a material that can switch textures and texture sets.

If you want to switch between more than two sets of textures, please see [Component:MultiTextureFader](https://wiki.resonite.com/Component:MultiTextureFader "Component:MultiTextureFader").

To see detailed info on the textures not unique to this material like albedo and specular, please see [Component:PBS\_Specular](https://wiki.resonite.com/Component:PBS_Specular "Component:PBS Specular").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `HighPriorityIntegration` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | If true, integrating this asset (e.g. processing procedural assets) gets higher priority than assets with this flag off. An example is user laser procedural meshes. |
| `_shader` | **[Shader](https://wiki.resonite.com/Type:Shader "Type:Shader")** | Internal. |
| `Lerp` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The value to use to transition between the first and second texture and value sets in absence of `LerpTexture`. |
| `LerpTexture` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | The texture to use to blend linearly between the first and second texture and value sets. |
| `LerpTextureScale` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The UV scale of the lerp texture. |
| `LerpTextureOffset` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The UV offset of the lerp texture. |
| `Texture0Scale` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The size of the `Texture0` on the surface. |
| `Texture0Offset` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The offset of the `Texture0` on the surface. |
| `Texture1Scale` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The size of the `Texture1` on the surface. |
| `Texture1Offset` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The offset of the `Texture1` on the surface. |
| `AlbedoColor0` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color tint of `Texture0`. |
| `AlbedoColor1` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color tint of `Texture1`. |
| `AlbedoTexture0` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | Texture 0 for albedo. |
| `AlbedoTexture1` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | Texture 1 for albedo. |
| `EmissiveColor0` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The emissive texture tint for texture 0. |
| `EmissiveColor1` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The emissive texture tint for texture 1. |
| `EmissiveMap0` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | The texture 0 for emissive. |
| `EmissiveMap1` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | The texture 1 for emissive. |
| `NormalMap0` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | The normal map for the first lerp texture set. |
| `NormalMap1` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | The normal map for the second lerp texture set. |
| `NormalScale0` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The normal scale for normal 0. |
| `NormalScale1` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The normal scale for normal 1. |
| `MultiValue` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Multiplies the constant value versions of packed texture information with the corrosponding channel of the packed image. |
| `OcclusionMap0` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | The occlusion map for texture 0. |
| `OcclusionMap1` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | The occlusion map for texture 1. |
| `BlendMode` | **[BlendMode](https://wiki.resonite.com/Type:BlendMode "Type:BlendMode")** | How to blend this material's colors vs what it rendered on top of. |
| `AlphaCutoff` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The minimum threshold for alpha which before this value it will be not rendered for that pixel. |
| `ZWrite` | **[ZWrite](https://wiki.resonite.com/Type:ZWrite "Type:ZWrite")** | whether this material should respect the distance it is from the camera. |
| `ZTest` | **[ZTest](https://wiki.resonite.com/Type:ZTest "Type:ZTest")** | Determines whether this object should render when it is in front of or behind other objects that respect depth from the camera |
| `Culling` | **[Culling](https://wiki.resonite.com/Type:Culling "Type:Culling")** | Whether to show the material on the front, back, or both sides |
| `OffsetFactor` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much this material should be pushed forwards or backwards on the depth buffer, based on the polygon's slope relative to the camera (i.e. polygons parallel to the camera will not be affected by this).[\[1\]](https://wiki.resonite.com/Component:PBSLerpSpecular#cite_note-Material_OffsetFactor/Units_Desc-1) |
| `OffsetUnits` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much this material should be pushed forwards or backwards on the depth buffer (regardless of the polygon's slope relative to the camera), in units equal to the smallest possible difference for the rendering device being used.[\[1\]](https://wiki.resonite.com/Component:PBSLerpSpecular#cite_note-Material_OffsetFactor/Units_Desc-1) |
| `RenderQueue` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | changes at which point a material renders on the render stack |
| `SpecularColor0` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color for the Specular for texture set 0. |
| `SpecularColor1` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color for the Specular for texture set 1. |
| `SpecularMap0` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | The map for the Specular for texture set 0. |
| `SpecularMap1` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | The map for the Specular for texture set 1. |

Fields
Collapse

## Usage

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Component:PBSLerpMetallic](https://wiki.resonite.com/Component:PBSLerpMetallic "Component:PBSLerpMetallic")
- [Component:MultiTextureFader](https://wiki.resonite.com/Component:MultiTextureFader "Component:MultiTextureFader")
- [Component:PBS\_Specular](https://wiki.resonite.com/Component:PBS_Specular "Component:PBS Specular")

1. ↑ [Jump up to: 1.0](https://wiki.resonite.com/Component:PBSLerpSpecular#cite_ref-Material_OffsetFactor/Units_Desc_1-0)[1.1](https://wiki.resonite.com/Component:PBSLerpSpecular#cite_ref-Material_OffsetFactor/Units_Desc_1-1)[https://docs.unity3d.com/6000.2/Documentation/Manual/SL-Offset.html](https://docs.unity3d.com/6000.2/Documentation/Manual/SL-Offset.html)

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:PBSLerpSpecular&oldid=105839](https://wiki.resonite.com/index.php?title=Component:PBSLerpSpecular&oldid=105839)"

Contents