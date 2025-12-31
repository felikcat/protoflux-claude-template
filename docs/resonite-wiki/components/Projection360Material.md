# Component:Projection360Material

> Source: https://wiki.resonite.com/Component:Projection360Material

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:Projection360Material&diff=106669) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/0/0f/Projection360MaterialComponent.png/510px-Projection360MaterialComponent.png)](https://wiki.resonite.com/File:Projection360MaterialComponent.png) **Projection360 Material** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `HighPriorityIntegration` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | If true, integrating this asset (e.g. processing procedural assets) gets higher priority than assets with this flag off. An example is user laser procedural meshes. |
| `_shader` | **[Shader](https://wiki.resonite.com/Type:Shader "Type:Shader")** | Internal. |
| `Texture` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | The texture to debug data for. |
| `SecondaryTexture` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | [Template:Material SecondaryTexture](https://wiki.resonite.com/index.php?title=Template:Material_SecondaryTexture&action=edit&redlink=1 "Template:Material SecondaryTexture (page does not exist)") |
| `Cubemap` | **[Cubemap](https://wiki.resonite.com/Type:Cubemap "Type:Cubemap")** | [Template:Material Cubemap](https://wiki.resonite.com/index.php?title=Template:Material_Cubemap&action=edit&redlink=1 "Template:Material Cubemap (page does not exist)") |
| `SecondaryCubemap` | **[Cubemap](https://wiki.resonite.com/Type:Cubemap "Type:Cubemap")** | [Template:Material SecondaryCubemap](https://wiki.resonite.com/index.php?title=Template:Material_SecondaryCubemap&action=edit&redlink=1 "Template:Material SecondaryCubemap (page does not exist)") |
| `CubemapLOD` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | [Template:Material CubemapLOD](https://wiki.resonite.com/index.php?title=Template:Material_CubemapLOD&action=edit&redlink=1 "Template:Material CubemapLOD (page does not exist)") |
| `TextureLerp` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | [Template:Material TextureLerp](https://wiki.resonite.com/index.php?title=Template:Material_TextureLerp&action=edit&redlink=1 "Template:Material TextureLerp (page does not exist)") |
| `Projection` | **[Mode](https://wiki.resonite.com/Component:Projection360Material#Mode)** | [Template:Material Projection](https://wiki.resonite.com/index.php?title=Template:Material_Projection&action=edit&redlink=1 "Template:Material Projection (page does not exist)") |
| `FieldOfView` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | the field of view of the `Depth` data. |
| `AngleOffset` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | [Template:Material AngleOffset](https://wiki.resonite.com/index.php?title=Template:Material_AngleOffset&action=edit&redlink=1 "Template:Material AngleOffset (page does not exist)") |
| `PerspectiveFieldOfView` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | [Template:Material PerspectiveFieldOfView](https://wiki.resonite.com/index.php?title=Template:Material_PerspectiveFieldOfView&action=edit&redlink=1 "Template:Material PerspectiveFieldOfView (page does not exist)") |
| `PerspectiveAngleOffset` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | [Template:Material PerspectiveAngleOffset](https://wiki.resonite.com/index.php?title=Template:Material_PerspectiveAngleOffset&action=edit&redlink=1 "Template:Material PerspectiveAngleOffset (page does not exist)") |
| `Tint` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color to multiply or tint by for the entire material. |
| `Exposure` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much exposure or brightness should be given to the sky. |
| `Gamma` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | the gamma effect. |
| `TintTexture` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | [Template:Material TintTexture](https://wiki.resonite.com/index.php?title=Template:Material_TintTexture&action=edit&redlink=1 "Template:Material TintTexture (page does not exist)") |
| `TintTextureScale` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | [Template:Material TintTextureScale](https://wiki.resonite.com/index.php?title=Template:Material_TintTextureScale&action=edit&redlink=1 "Template:Material TintTextureScale (page does not exist)") |
| `TintTextureOffset` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | [Template:Material TintTextureOffset](https://wiki.resonite.com/index.php?title=Template:Material_TintTextureOffset&action=edit&redlink=1 "Template:Material TintTextureOffset (page does not exist)") |
| `TintTextureMode` | **[TintMode](https://wiki.resonite.com/Component:Projection360Material#TintMode)** | [Template:Material TintTextureMode](https://wiki.resonite.com/index.php?title=Template:Material_TintTextureMode&action=edit&redlink=1 "Template:Material TintTextureMode (page does not exist)") |
| `Tint0` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | [Template:Material Tint0](https://wiki.resonite.com/index.php?title=Template:Material_Tint0&action=edit&redlink=1 "Template:Material Tint0 (page does not exist)") |
| `Tint1` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | [Template:Material Tint1](https://wiki.resonite.com/index.php?title=Template:Material_Tint1&action=edit&redlink=1 "Template:Material Tint1 (page does not exist)") |
| `OutsideMode` | **[Outside](https://wiki.resonite.com/Component:Projection360Material#Outside)** | [Template:Material OutsideMode](https://wiki.resonite.com/index.php?title=Template:Material_OutsideMode&action=edit&redlink=1 "Template:Material OutsideMode (page does not exist)") |
| `OutsideColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | [Template:Material OutsideColor](https://wiki.resonite.com/index.php?title=Template:Material_OutsideColor&action=edit&redlink=1 "Template:Material OutsideColor (page does not exist)") |
| `TextureOffset` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | How much to shift around the position of the different texture maps. |
| `TextureScale` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | How much to scale up or down the different texture maps. |
| `StereoTextureTransform` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether a texture on the surface should appear different in the right eye. |
| `RightEyeTextureOffset` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The override for texture in the right eye for offset. |
| `RightEyeTextureScale` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The override for texture in the right eye for scale. |
| `Sidedness` | **[Sidedness](https://wiki.resonite.com/Type:Sidedness "Type:Sidedness")** | Render on both sides of the mesh, front, or back. |
| `ZWrite` | **[ZWrite](https://wiki.resonite.com/Type:ZWrite "Type:ZWrite")** | whether this material should respect the distance it is from the camera. |
| `ZTest` | **[ZTest](https://wiki.resonite.com/Type:ZTest "Type:ZTest")** | Determines whether this object should render when it is in front of or behind other objects that respect depth from the camera |
| `BlendMode` | **[BlendMode](https://wiki.resonite.com/Type:BlendMode "Type:BlendMode")** | How to blend this material's colors vs what it rendered on top of. |
| `OffsetFactor` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much this material should be pushed forwards or backwards on the depth buffer, based on the polygon's slope relative to the camera (i.e. polygons parallel to the camera will not be affected by this).[\[1\]](https://wiki.resonite.com/Component:Projection360Material#cite_note-Material_OffsetFactor/Units_Desc-1) |
| `OffsetUnits` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much this material should be pushed forwards or backwards on the depth buffer (regardless of the polygon's slope relative to the camera), in units equal to the smallest possible difference for the rendering device being used.[\[1\]](https://wiki.resonite.com/Component:Projection360Material#cite_note-Material_OffsetFactor/Units_Desc-1) |
| `MaxIntensity` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | [Template:Material MaxIntensity](https://wiki.resonite.com/index.php?title=Template:Material_MaxIntensity&action=edit&redlink=1 "Template:Material MaxIntensity (page does not exist)") |
| `Rect` | **[Rect](https://wiki.resonite.com/Type:Rect "Type:Rect")** | See [RectClip on Materials](https://wiki.resonite.com/RectClip_on_Materials "RectClip on Materials"). |
| `RectClip` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Toggles if the material should use `Rect` |
| `ColorMask` | **[ColorMask](https://wiki.resonite.com/Type:ColorMask "Type:ColorMask")** | What colors behind the material should make it through the filter. |
| `OffsetTexture` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | The texture used to offset the positions of pixels. |
| `OffsetMask` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | [Template:Material OffsetMask](https://wiki.resonite.com/index.php?title=Template:Material_OffsetMask&action=edit&redlink=1 "Template:Material OffsetMask (page does not exist)") |
| `OffsetTextureOffset` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | How much to offset the detail of the `OffsetTexture` |
| `OffsetTextureScale` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | How much to scale the detail of the `OffsetTexture` |
| `OffsetMagnitude` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | How much to amplify the offset effect. |
| `StencilComparison` | **[StencilComparison](https://wiki.resonite.com/Type:StencilComparison "Type:StencilComparison")** | See [Type:StencilComparison](https://wiki.resonite.com/Type:StencilComparison "Type:StencilComparison") for an in depth explanation on what this does. |
| `StencilOperation` | **[StencilOperation](https://wiki.resonite.com/Type:StencilOperation "Type:StencilOperation")** | See [Type:StencilOperation](https://wiki.resonite.com/Type:StencilOperation "Type:StencilOperation") for an in depth explanation on what this does. |
| `StencilID` | **[Byte](https://wiki.resonite.com/Type:Byte "Type:Byte")** | The Stencil ID of this material. This is sometimes written to the frame buffer's [Stencil](https://wiki.resonite.com/Stencil "Stencil") mask, or used to determine whether this material should render for a particular pixel. |
| `StencilWriteMask` | **[Byte](https://wiki.resonite.com/Type:Byte "Type:Byte")** | does a Bitwise AND with this number for every pixel in the frame buffer this is rendering on top of when this object is drawn, after reading from the buffer. |
| `StencilReadMask` | **[Byte](https://wiki.resonite.com/Type:Byte "Type:Byte")** | is bitwise ANDed with the [Stencil](https://wiki.resonite.com/Stencil "Stencil") in the frame buffer before the test compares them. |
| `RenderQueue` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | changes at which point a material renders on the render stack |

Fields
Collapse

## Mode

| Name | Value | Description |
| --- | --- | --- |

Values

## OutsideMode

| Name | Value | Description |
| --- | --- | --- |

Values

## TintMode

| Name | Value | Description |
| --- | --- | --- |

Values

## Usage

## Examples

## See Also

1. ↑ [Jump up to: 1.0](https://wiki.resonite.com/Component:Projection360Material#cite_ref-Material_OffsetFactor/Units_Desc_1-0)[1.1](https://wiki.resonite.com/Component:Projection360Material#cite_ref-Material_OffsetFactor/Units_Desc_1-1)[https://docs.unity3d.com/6000.2/Documentation/Manual/SL-Offset.html](https://docs.unity3d.com/6000.2/Documentation/Manual/SL-Offset.html)

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:Projection360Material&oldid=106669](https://wiki.resonite.com/index.php?title=Component:Projection360Material&oldid=106669)"

Contents