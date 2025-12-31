# Component:ChannelMatrixMaterial

> Source: https://wiki.resonite.com/Component:ChannelMatrixMaterial

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:ChannelMatrixMaterial&diff=105819) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/0/0c/ChannelMatrixMaterialComponent.png/510px-ChannelMatrixMaterialComponent.png)](https://wiki.resonite.com/File:ChannelMatrixMaterialComponent.png) **Channel Matrix Material** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ChannelMatrixMaterial** component can be used to make meshes render the colors behind them differently by mixing around the color channels of colors behind them.

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
| `RedFromRed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much should be added to the resulting red color from the original red channel |
| `RedFromGreen` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much should be added to the resulting red color from the original green channel |
| `RedFromBlue` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much should be added to the resulting red color from the original blue channel |
| `RedOffset` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | how much to add to the resulting red color. |
| `GreenFromRed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much should be added to the resulting green color from the original red channel |
| `GreenFromGreen` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much should be added to the resulting green color from the original green channel |
| `GreenFromBlue` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much should be added to the resulting green color from the original blue channel |
| `GreenOffset` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | how much to add to the resulting green color. |
| `BlueFromRed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much should be added to the resulting blue color from the original red channel |
| `BlueFromGreen` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much should be added to the resulting blue color from the original green channel |
| `BlueFromBlue` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much should be added to the resulting blue color from the original blue channel |
| `BlueOffset` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | how much to add to the resulting blue color. |
| `ClampRedMin` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | the minimum resulting red color. |
| `ClampGreenMin` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | the minimum resulting green color |
| `ClampBlueMin` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | the minimum resulting blue color |
| `ClampRedMax` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | the maximum resulting red color. |
| `ClampGreenMax` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | the maximum resulting green color |
| `ClampBlueMax` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | the maximum resulting blue color |
| `BlendMode` | **[BlendMode](https://wiki.resonite.com/Type:BlendMode "Type:BlendMode")** | How to blend this material's colors vs what it rendered on top of. |
| `Sidedness` | **[Sidedness](https://wiki.resonite.com/Type:Sidedness "Type:Sidedness")** | Render on both sides of the mesh, front, or back. |
| `ZWrite` | **[ZWrite](https://wiki.resonite.com/Type:ZWrite "Type:ZWrite")** | whether this material should respect the distance it is from the camera. |
| `ZTest` | **[ZTest](https://wiki.resonite.com/Type:ZTest "Type:ZTest")** | Determines whether this object should render when it is in front of or behind other objects that respect depth from the camera |

Fields
Collapse

## Usage

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ChannelMatrixMaterial&oldid=105819](https://wiki.resonite.com/index.php?title=Component:ChannelMatrixMaterial&oldid=105819)"

Contents