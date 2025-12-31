# Component:UnlitMaterial

> Source: https://wiki.resonite.com/Component:UnlitMaterial

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:UnlitMaterial&diff=105880) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/1/1a/UnlitMaterialComponent.png/510px-UnlitMaterialComponent.png)](https://wiki.resonite.com/File:UnlitMaterialComponent.png) **Unlit Material** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **UnlitMaterial** component is a material that can render meshes without lighting at full bright. Optionally can render each vertex like a square that faces the user or a direction. It can also optionally render differently depending on which eye it is viewed from. This is used in the left and right cat item, and for 3D photos.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `HighPriorityIntegration` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | If true, integrating this asset (e.g. processing procedural assets) gets higher priority than assets with this flag off. An example is user laser procedural meshes. |
| `TintColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | What color to tint the projected image. |
| `Texture` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | The texture to debug data for. |
| `TextureScale` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | How much to scale up or down the different texture maps. |
| `TextureOffset` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | How much to shift around the position of the different texture maps. |
| `MaskTexture` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | The mask texture to use. |
| `MaskScale` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The UV scale of the mask texture. |
| `MaskOffset` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The UV offset of the mask texture. |
| `MaskMode` | **[MaskTextureMode](https://wiki.resonite.com/Type:MaskTextureMode "Type:MaskTextureMode")** | How to apply the mask texture to the material. |
| `BlendMode` | **[BlendMode](https://wiki.resonite.com/Type:BlendMode "Type:BlendMode")** | How to blend this material's colors vs what it rendered on top of. |
| `AlphaCutoff` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | If `BlendMode` is set to cutout, discard rendering of pixels for the surface that fall below this alpha threshold. |
| `UseVertexColors` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the material should use vertex colors from the mesh. |
| `VertexColorInterpolationSpace` | **[ColorProfile](https://wiki.resonite.com/Type:ColorProfile "Type:ColorProfile")** | How to interpolate vertex colors on the mesh. |
| `Sidedness` | **[Sidedness](https://wiki.resonite.com/Type:Sidedness "Type:Sidedness")** | Render on both sides of the mesh, front, or back. |
| `ZWrite` | **[ZWrite](https://wiki.resonite.com/Type:ZWrite "Type:ZWrite")** | whether this material should respect the distance it is from the camera. |
| `OffsetTexture` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | The texture used to offset the positions of pixels. |
| `OffsetMagnitude` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | How much to amplify the offset effect. |
| `OffsetTextureScale` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | How much to scale the detail of the `OffsetTexture` |
| `OffsetTextureOffset` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | How much to offset the detail of the `OffsetTexture` |
| `PolarUVmapping` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to use polar UV unwrapping. |
| `PolarPower` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The power of the polar UV unwrapping. |
| `StereoTextureTransform` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether a texture on the surface should appear different in the right eye. |
| `RightEyeTextureScale` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The override for texture in the right eye for scale. |
| `RightEyeTextureOffset` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The override for texture in the right eye for offset. |
| `DecodeAsNormalMap` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to decode the textures as a normal map. |
| `UseBillboardGeometry` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to not render the surface, and instead render each vertex like a Particle with this material and texture. |
| `UsePerBillboardScale` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether scaling of vertex points should be used for Billboard geometry positioning. |
| `UsePerBillboardRotation` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether rotation of vertex points should be used for Billboard geometry positioning. |
| `UsePerBillboardUV` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether uv data of vertex points should be used for Billboard geometry positioning. |
| `BillboardSize` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The base size for Billboard geometry. |
| `OffsetFactor` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much this material should be pushed forwards or backwards on the depth buffer, based on the polygon's slope relative to the camera (i.e. polygons parallel to the camera will not be affected by this).[\[1\]](https://wiki.resonite.com/Component:UnlitMaterial#cite_note-Material_OffsetFactor/Units_Desc-1) |
| `OffsetUnits` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much this material should be pushed forwards or backwards on the depth buffer (regardless of the polygon's slope relative to the camera), in units equal to the smallest possible difference for the rendering device being used.[\[1\]](https://wiki.resonite.com/Component:UnlitMaterial#cite_note-Material_OffsetFactor/Units_Desc-1) |
| `RenderQueue` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | changes at which point a material renders on the render stack |
| `_unlit` | **[Shader](https://wiki.resonite.com/Type:Shader "Type:Shader")** | [Template:Material unlit](https://wiki.resonite.com/index.php?title=Template:Material_unlit&action=edit&redlink=1 "Template:Material unlit (page does not exist)") |
| `_unlitBillboard` | **[Shader](https://wiki.resonite.com/Type:Shader "Type:Shader")** | [Template:Material unlitBillboard](https://wiki.resonite.com/index.php?title=Template:Material_unlitBillboard&action=edit&redlink=1 "Template:Material unlitBillboard (page does not exist)") |

Fields
Collapse

## Usage

Attach to a slot and use the material Component in the list of materials on a [Component:MeshRenderer](https://wiki.resonite.com/Component:MeshRenderer "Component:MeshRenderer") or a [Component:SkinnedMeshRenderer](https://wiki.resonite.com/Component:SkinnedMeshRenderer "Component:SkinnedMeshRenderer") with a mesh to view what this material looks like.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

1. ↑ [Jump up to: 1.0](https://wiki.resonite.com/Component:UnlitMaterial#cite_ref-Material_OffsetFactor/Units_Desc_1-0)[1.1](https://wiki.resonite.com/Component:UnlitMaterial#cite_ref-Material_OffsetFactor/Units_Desc_1-1)[https://docs.unity3d.com/6000.2/Documentation/Manual/SL-Offset.html](https://docs.unity3d.com/6000.2/Documentation/Manual/SL-Offset.html)

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:UnlitMaterial&oldid=105880](https://wiki.resonite.com/index.php?title=Component:UnlitMaterial&oldid=105880)"

Contents