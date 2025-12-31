# Component:OverlayUnlitMaterial

> Source: https://wiki.resonite.com/Component:OverlayUnlitMaterial

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:OverlayUnlitMaterial&diff=105837) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/1/1b/OverlayUnlitMaterialComponent.png/510px-OverlayUnlitMaterialComponent.png)](https://wiki.resonite.com/File:OverlayUnlitMaterialComponent.png) **Overlay Unlit Material** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **OverlayUnlitMaterial** component is a material that is similar to a [Component:UnlitMaterial](https://wiki.resonite.com/Component:UnlitMaterial "Component:UnlitMaterial") except it renders differently when in front or behind an object.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `HighPriorityIntegration` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | If true, integrating this asset (e.g. processing procedural assets) gets higher priority than assets with this flag off. An example is user laser procedural meshes. |
| `_shader` | **[Shader](https://wiki.resonite.com/Type:Shader "Type:Shader")** | Internal. |
| `BehindTintColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color tint when the material is behind an object. |
| `FrontTintColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color tint when the material is in front of an object. |
| `BehindTexture` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | The texture to use when the material is behind an object. |
| `BehindTextureScale` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The UV scale of `BehindTexture`. |
| `BehindTextureOffset` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The UV offset of `BehindTexture`. |
| `FrontTexture` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | The texture to use when the material is in front of an object. |
| `FrontTextureScale` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The UV scale of `FrontTexture`. |
| `FrontTextureOffset` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The UV offset of `FrontTexture`. |
| `BlendMode` | **[BlendMode](https://wiki.resonite.com/Type:BlendMode "Type:BlendMode")** | How to blend this material's colors vs what it rendered on top of. |
| `AlphaCutoff` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | If `BlendMode` is set to cutout, discard rendering of pixels for the surface that fall below this alpha threshold. |
| `UseVertexColors` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the material should use vertex colors from the mesh. |
| `VertexColorInterpolationSpace` | **[ColorProfile](https://wiki.resonite.com/Type:ColorProfile "Type:ColorProfile")** | How to interpolate vertex colors on the mesh. |
| `Sidedness` | **[Sidedness](https://wiki.resonite.com/Type:Sidedness "Type:Sidedness")** | Render on both sides of the mesh, front, or back. |
| `ZWrite` | **[ZWrite](https://wiki.resonite.com/Type:ZWrite "Type:ZWrite")** | whether this material should respect the distance it is from the camera. |
| `PolarUVmapping` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to use polar UV unwrapping. |
| `PolarPower` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The power of the polar UV unwrapping. |
| `OffsetFactor` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much this material should be pushed forwards or backwards on the depth buffer, based on the polygon's slope relative to the camera (i.e. polygons parallel to the camera will not be affected by this).[\[1\]](https://wiki.resonite.com/Component:OverlayUnlitMaterial#cite_note-Material_OffsetFactor/Units_Desc-1) |
| `OffsetUnits` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much this material should be pushed forwards or backwards on the depth buffer (regardless of the polygon's slope relative to the camera), in units equal to the smallest possible difference for the rendering device being used.[\[1\]](https://wiki.resonite.com/Component:OverlayUnlitMaterial#cite_note-Material_OffsetFactor/Units_Desc-1) |
| `RenderQueue` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | changes at which point a material renders on the render stack |

Fields
Collapse

## Usage

Attach to a slot and put into the materials of a renderer like a [Component:SkinnedMeshRenderer](https://wiki.resonite.com/Component:SkinnedMeshRenderer "Component:SkinnedMeshRenderer") or a [Component:MeshRenderer](https://wiki.resonite.com/Component:MeshRenderer "Component:MeshRenderer") with a mesh to view what the material looks like.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

1. ↑ [Jump up to: 1.0](https://wiki.resonite.com/Component:OverlayUnlitMaterial#cite_ref-Material_OffsetFactor/Units_Desc_1-0)[1.1](https://wiki.resonite.com/Component:OverlayUnlitMaterial#cite_ref-Material_OffsetFactor/Units_Desc_1-1)[https://docs.unity3d.com/6000.2/Documentation/Manual/SL-Offset.html](https://docs.unity3d.com/6000.2/Documentation/Manual/SL-Offset.html)

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:OverlayUnlitMaterial&oldid=105837](https://wiki.resonite.com/index.php?title=Component:OverlayUnlitMaterial&oldid=105837)"

Contents