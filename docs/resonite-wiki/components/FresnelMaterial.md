# Component:FresnelMaterial

> Source: https://wiki.resonite.com/Component:FresnelMaterial

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:FresnelMaterial&diff=105826) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/1/13/FresnelMaterialComponent.png/510px-FresnelMaterialComponent.png)](https://wiki.resonite.com/File:FresnelMaterialComponent.png) **Fresnel Material** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **FresnelLerpMaterial** component is a material that can be used to make a fresnel effect.

Far on this material is the geometry facing away from the camera and near is the geometry facing towards the camera.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `HighPriorityIntegration` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | If true, integrating this asset (e.g. processing procedural assets) gets higher priority than assets with this flag off. An example is user laser procedural meshes. |
| `_shader` | **[Shader](https://wiki.resonite.com/Type:Shader "Type:Shader")** | Internal. |
| `Exponent` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The sharpness of the fresnel effect. |
| `GammaCurve` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The gamma curve of the material colors. |
| `FarColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color tint of geometry facing away from the camera. |
| `NearColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color tint of geometry facing towards the camera. |
| `FarTexture` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | The texture for the geometry facing away from the camera. |
| `NearTexture` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | The texture for geometry facing towards the camera. |
| `FarTextureScale` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The UV scale of the far texture. |
| `FarTextureOffset` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The UV offset of the far texture. |
| `NearTextureScale` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The UV scale of the near texture. |
| `NearTextureOffset` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The UV offset of the near texture. |
| `NormalMap` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | The normal map is used as a way to change the appearance of a surface when shined on by lights, to give the illusion of a raised surface. |
| `NormalScale` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to scale up the effect of the normal map. |
| `UseVertexColors` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the material should use vertex colors from the mesh. |
| `VertexColorInterpolationSpace` | **[ColorProfile](https://wiki.resonite.com/Type:ColorProfile "Type:ColorProfile")** | How to interpolate vertex colors on the mesh. |
| `BlendMode` | **[BlendMode](https://wiki.resonite.com/Type:BlendMode "Type:BlendMode")** | How to blend this material's colors vs what it rendered on top of. |
| `AlphaCutoff` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | If `BlendMode` is set to cutout, discard rendering of pixels for the surface that fall below this alpha threshold. |
| `MaskTexture` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | The mask texture to use. |
| `MaskScale` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The UV scale of the mask texture. |
| `MaskOffset` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The UV offset of the mask texture. |
| `MaskMode` | **[MaskTextureMode](https://wiki.resonite.com/Type:MaskTextureMode "Type:MaskTextureMode")** | How to apply the mask texture to the material. |
| `Sidedness` | **[Sidedness](https://wiki.resonite.com/Type:Sidedness "Type:Sidedness")** | Render on both sides of the mesh, front, or back. |
| `ZWrite` | **[ZWrite](https://wiki.resonite.com/Type:ZWrite "Type:ZWrite")** | whether this material should respect the distance it is from the camera. |
| `ZTest` | **[ZTest](https://wiki.resonite.com/Type:ZTest "Type:ZTest")** | Determines whether this object should render when it is in front of or behind other objects that respect depth from the camera |
| `OffsetFactor` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much this material should be pushed forwards or backwards on the depth buffer, based on the polygon's slope relative to the camera (i.e. polygons parallel to the camera will not be affected by this).[\[1\]](https://wiki.resonite.com/Component:FresnelMaterial#cite_note-Material_OffsetFactor/Units_Desc-1) |
| `OffsetUnits` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much this material should be pushed forwards or backwards on the depth buffer (regardless of the polygon's slope relative to the camera), in units equal to the smallest possible difference for the rendering device being used.[\[1\]](https://wiki.resonite.com/Component:FresnelMaterial#cite_note-Material_OffsetFactor/Units_Desc-1) |
| `RenderQueue` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | changes at which point a material renders on the render stack |
| `PolarUVmapping` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to use polar UV unwrapping. |
| `PolarPower` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The power of the polar UV unwrapping. |

Fields
Collapse

## Usage

Attach to a slot and put into the materials of a renderer like a [Component:SkinnedMeshRenderer](https://wiki.resonite.com/Component:SkinnedMeshRenderer "Component:SkinnedMeshRenderer") or a [Component:MeshRenderer](https://wiki.resonite.com/Component:MeshRenderer "Component:MeshRenderer") with a mesh to view what the material looks like.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

1. ↑ [Jump up to: 1.0](https://wiki.resonite.com/Component:FresnelMaterial#cite_ref-Material_OffsetFactor/Units_Desc_1-0)[1.1](https://wiki.resonite.com/Component:FresnelMaterial#cite_ref-Material_OffsetFactor/Units_Desc_1-1)[https://docs.unity3d.com/6000.2/Documentation/Manual/SL-Offset.html](https://docs.unity3d.com/6000.2/Documentation/Manual/SL-Offset.html)

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:FresnelMaterial&oldid=105826](https://wiki.resonite.com/index.php?title=Component:FresnelMaterial&oldid=105826)"

Contents