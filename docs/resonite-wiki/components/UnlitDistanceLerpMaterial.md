# Component:UnlitDistanceLerpMaterial

> Source: https://wiki.resonite.com/Component:UnlitDistanceLerpMaterial

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:UnlitDistanceLerpMaterial&diff=105879) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/6/6d/UnlitDistanceLerpMaterialComponent.png/510px-UnlitDistanceLerpMaterialComponent.png)](https://wiki.resonite.com/File:UnlitDistanceLerpMaterialComponent.png) **Unlit Distance Lerp Material** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **UnlitDistanceLerpMaterial** component changes it's surface depending on how close the material's surface is to a given `Point`.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `HighPriorityIntegration` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | If true, integrating this asset (e.g. processing procedural assets) gets higher priority than assets with this flag off. An example is user laser procedural meshes. |
| `_shader` | **[Shader](https://wiki.resonite.com/Type:Shader "Type:Shader")** | Internal. |
| `LocalSpace` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to calculate `Distance` and `Point` in local space. |
| `Point` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The point to measure from. |
| `Distance` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The distance where the transition from near to far starts. |
| `TransitionRange` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much distance from near, far is. |
| `NearTexture` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | The texture for geometry facing towards the camera. |
| `FarTexture` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | The texture for the geometry facing away from the camera. |
| `NearTextureScale` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The UV scale of the near texture. |
| `NearTextureOffset` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The UV offset of the near texture. |
| `FarTextureScale` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The UV scale of the far texture. |
| `FarTextureOffset` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The UV offset of the far texture. |
| `NearColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color tint of geometry facing towards the camera. |
| `FarColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color tint of geometry facing away from the camera. |
| `UseVertexColors` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the material should use vertex colors from the mesh. |
| `VertexColorInterpolationSpace` | **[ColorProfile](https://wiki.resonite.com/Type:ColorProfile "Type:ColorProfile")** | How to interpolate vertex colors on the mesh. |
| `BlendMode` | **[BlendMode](https://wiki.resonite.com/Type:BlendMode "Type:BlendMode")** | How to blend this material's colors vs what it rendered on top of. |
| `AlphaCutoff` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | If `BlendMode` is set to cutout, discard rendering of pixels for the surface that fall below this alpha threshold. |
| `Sidedness` | **[Sidedness](https://wiki.resonite.com/Type:Sidedness "Type:Sidedness")** | Render on both sides of the mesh, front, or back. |
| `ZWrite` | **[ZWrite](https://wiki.resonite.com/Type:ZWrite "Type:ZWrite")** | whether this material should respect the distance it is from the camera. |
| `OffsetFactor` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much this material should be pushed forwards or backwards on the depth buffer, based on the polygon's slope relative to the camera (i.e. polygons parallel to the camera will not be affected by this).[\[1\]](https://wiki.resonite.com/Component:UnlitDistanceLerpMaterial#cite_note-Material_OffsetFactor/Units_Desc-1) |
| `OffsetUnits` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much this material should be pushed forwards or backwards on the depth buffer (regardless of the polygon's slope relative to the camera), in units equal to the smallest possible difference for the rendering device being used.[\[1\]](https://wiki.resonite.com/Component:UnlitDistanceLerpMaterial#cite_note-Material_OffsetFactor/Units_Desc-1) |
| `RenderQueue` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | changes at which point a material renders on the render stack |

Fields
Collapse

## Usage

Attach to a slot and use the material Component in the list of materials on a [Component:MeshRenderer](https://wiki.resonite.com/Component:MeshRenderer "Component:MeshRenderer") or a [Component:SkinnedMeshRenderer](https://wiki.resonite.com/Component:SkinnedMeshRenderer "Component:SkinnedMeshRenderer") with a mesh to view what this material looks like.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

1. ↑ [Jump up to: 1.0](https://wiki.resonite.com/Component:UnlitDistanceLerpMaterial#cite_ref-Material_OffsetFactor/Units_Desc_1-0)[1.1](https://wiki.resonite.com/Component:UnlitDistanceLerpMaterial#cite_ref-Material_OffsetFactor/Units_Desc_1-1)[https://docs.unity3d.com/6000.2/Documentation/Manual/SL-Offset.html](https://docs.unity3d.com/6000.2/Documentation/Manual/SL-Offset.html)

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:UnlitDistanceLerpMaterial&oldid=105879](https://wiki.resonite.com/index.php?title=Component:UnlitDistanceLerpMaterial&oldid=105879)"

Contents