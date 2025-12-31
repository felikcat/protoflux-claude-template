# Component:FresnelLerpMaterial

> Source: https://wiki.resonite.com/Component:FresnelLerpMaterial

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:FresnelLerpMaterial&diff=105825) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/0/0f/FresnelLerpMaterialComponent.png/510px-FresnelLerpMaterialComponent.png)](https://wiki.resonite.com/File:FresnelLerpMaterialComponent.png) **Fresnel Lerp Material** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **FresnelLerpMaterial** component is a material that can be used to make a fresnel effect that can be lerped between two different preset frensel settings.

Far on this material is the geometry facing away from the camera and near is the geometry facing towards the camera.

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
| `LerpTexturePolarUV` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to UV map the lerp texture using polar UVs. |
| `LerpTexturePolarPower` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The polar UV power of the lerp texture UV when using polar UVs. |
| `Exponent0` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The sharpness of the fresnel effect for the first lerp value set. |
| `Exponent1` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The sharpness of the fresnel effect for the second lerp value set. |
| `GammaCurve` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The gamma curve of the material colors. |
| `FarColor0` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The far color tint for the first lerp set. |
| `NearColor0` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The near color tint for the first lerp set. |
| `FarColor1` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The Far color tint for the second lerp set. |
| `NearColor1` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The near color tint for the second lerp set. |
| `FarTexture0` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | The Far texture for the first lerp texture set. |
| `NearTexture0` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | The near texture for the first lerp texture set. |
| `FarTexture1` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | The Far texture for the second lerp texture set. |
| `NearTexture1` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | The near texture for the second lerp texture set. |
| `NormalMap0` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | The normal map for the first lerp texture set. |
| `NormalMap1` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | The normal map for the second lerp texture set. |
| `BlendMode` | **[BlendMode](https://wiki.resonite.com/Type:BlendMode "Type:BlendMode")** | How to blend this material's colors vs what it rendered on top of. |
| `Sidedness` | **[Sidedness](https://wiki.resonite.com/Type:Sidedness "Type:Sidedness")** | Render on both sides of the mesh, front, or back. |
| `ZWrite` | **[ZWrite](https://wiki.resonite.com/Type:ZWrite "Type:ZWrite")** | whether this material should respect the distance it is from the camera. |
| `OffsetFactor` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much this material should be pushed forwards or backwards on the depth buffer, based on the polygon's slope relative to the camera (i.e. polygons parallel to the camera will not be affected by this).[\[1\]](https://wiki.resonite.com/Component:FresnelLerpMaterial#cite_note-Material_OffsetFactor/Units_Desc-1) |
| `OffsetUnits` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much this material should be pushed forwards or backwards on the depth buffer (regardless of the polygon's slope relative to the camera), in units equal to the smallest possible difference for the rendering device being used.[\[1\]](https://wiki.resonite.com/Component:FresnelLerpMaterial#cite_note-Material_OffsetFactor/Units_Desc-1) |
| `RenderQueue` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | changes at which point a material renders on the render stack |

Fields
Collapse

## Usage

Attach to a slot and put into the materials of a renderer like a [Component:SkinnedMeshRenderer](https://wiki.resonite.com/Component:SkinnedMeshRenderer "Component:SkinnedMeshRenderer") or a [Component:MeshRenderer](https://wiki.resonite.com/Component:MeshRenderer "Component:MeshRenderer") with a mesh to view what the material looks like.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

1. ↑ [Jump up to: 1.0](https://wiki.resonite.com/Component:FresnelLerpMaterial#cite_ref-Material_OffsetFactor/Units_Desc_1-0)[1.1](https://wiki.resonite.com/Component:FresnelLerpMaterial#cite_ref-Material_OffsetFactor/Units_Desc_1-1)[https://docs.unity3d.com/6000.2/Documentation/Manual/SL-Offset.html](https://docs.unity3d.com/6000.2/Documentation/Manual/SL-Offset.html)

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:FresnelLerpMaterial&oldid=105825](https://wiki.resonite.com/index.php?title=Component:FresnelLerpMaterial&oldid=105825)"

Contents