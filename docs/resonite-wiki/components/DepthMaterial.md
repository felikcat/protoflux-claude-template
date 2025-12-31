# Component:DepthMaterial

> Source: https://wiki.resonite.com/Component:DepthMaterial

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:DepthMaterial&diff=105821) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/5/50/DepthMaterialComponent.png/510px-DepthMaterialComponent.png)](https://wiki.resonite.com/File:DepthMaterialComponent.png) **Depth Material** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **DepthMaterial** component renders everything behind it in black and white depending on how far away it is from the camera.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `HighPriorityIntegration` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | If true, integrating this asset (e.g. processing procedural assets) gets higher priority than assets with this flag off. An example is user laser procedural meshes. |
| `Rect` | **[Rect](https://wiki.resonite.com/Type:Rect "Type:Rect")** | See [RectClip on Materials](https://wiki.resonite.com/RectClip_on_Materials "RectClip on Materials"). |
| `RectClip` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Toggles if the material should use `Rect` |
| `ColorMask` | **[ColorMask](https://wiki.resonite.com/Type:ColorMask "Type:ColorMask")** | What colors behind the material should make it through the filter. |
| `StencilComparison` | **[StencilComparison](https://wiki.resonite.com/Type:StencilComparison "Type:StencilComparison")** | See [Type:StencilComparison](https://wiki.resonite.com/Type:StencilComparison "Type:StencilComparison") for an in depth explanation on what this does. |
| `StencilOperation` | **[StencilOperation](https://wiki.resonite.com/Type:StencilOperation "Type:StencilOperation")** | See [Type:StencilOperation](https://wiki.resonite.com/Type:StencilOperation "Type:StencilOperation") for an in depth explanation on what this does. |
| `StencilID` | **[Byte](https://wiki.resonite.com/Type:Byte "Type:Byte")** | The Stencil ID of this material. This is sometimes written to the frame buffer's [Stencil](https://wiki.resonite.com/Stencil "Stencil") mask, or used to determine whether this material should render for a particular pixel. |
| `StencilWriteMask` | **[Byte](https://wiki.resonite.com/Type:Byte "Type:Byte")** | does a Bitwise AND with this number for every pixel in the frame buffer this is rendering on top of when this object is drawn, after reading from the buffer. |
| `StencilReadMask` | **[Byte](https://wiki.resonite.com/Type:Byte "Type:Byte")** | is bitwise ANDed with the [Stencil](https://wiki.resonite.com/Stencil "Stencil") in the frame buffer before the test compares them. |
| `RenderQueue` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | changes at which point a material renders on the render stack |
| `_shader` | **[Shader](https://wiki.resonite.com/Type:Shader "Type:Shader")** | Internal. |
| `Multiply` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | how much to multiply the resulting color. |
| `Offset` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to offset the positions of the displayed color data pixels. |
| `Clip` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | whether to clip the depth range. |
| `ClipStart` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | the depth start value, which is the minimum distance from the camera which will be black. |
| `ClipEnd` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | the depth end value, which is the maximum distance from the camera, which will be white. |
| `BlendMode` | **[BlendMode](https://wiki.resonite.com/Type:BlendMode "Type:BlendMode")** | How to blend this material's colors vs what it rendered on top of. |
| `Sidedness` | **[Sidedness](https://wiki.resonite.com/Type:Sidedness "Type:Sidedness")** | Render on both sides of the mesh, front, or back. |
| `ZWrite` | **[ZWrite](https://wiki.resonite.com/Type:ZWrite "Type:ZWrite")** | whether this material should respect the distance it is from the camera. |
| `ZTest` | **[ZTest](https://wiki.resonite.com/Type:ZTest "Type:ZTest")** | Determines whether this object should render when it is in front of or behind other objects that respect depth from the camera |

Fields
Collapse

## Usage

Attach to a slot and apply to a [Component:MeshRenderer](https://wiki.resonite.com/Component:MeshRenderer "Component:MeshRenderer") or [Component:SkinnedMeshRenderer](https://wiki.resonite.com/Component:SkinnedMeshRenderer "Component:SkinnedMeshRenderer") to see the visual effect this component makes.

## Examples

Can be used to make a blindess or sonar effect.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:DepthMaterial&oldid=105821](https://wiki.resonite.com/index.php?title=Component:DepthMaterial&oldid=105821)"

Contents