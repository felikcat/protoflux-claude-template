# Component:BlurMaterial

> Source: https://wiki.resonite.com/Component:BlurMaterial

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:BlurMaterial&diff=105818) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/c/c9/BlurMaterialComponent.png/510px-BlurMaterialComponent.png)](https://wiki.resonite.com/File:BlurMaterialComponent.png) **Blur Material** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **BlurMaterial** Component is used to blur objects rendered behind it, by first rendering everything behind it using z-test and then grabbing the pixels, then creating spread transparent ghost images of the original pixels to give the illusion of blur.

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
| `Iterations` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | How many ghost images to make in order to incur the blurring effect |
| `Spread` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | How much the ghost images spread from the center real image to incur the blurring effect |
| `SpreadMagnitudeTexture` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | A texture to use that affects the strength of the blur effect. |
| `UsePoissonDisc` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Use the poisson disk blur algorithm |
| `DepthFadeDivisor` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | This setting uses the depth of the scene as a scaling factor for how blurry the filter is based on this depth, so further out objects get more blurry. |
| `SpreadTextureScale` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The uv scale of the `SpreadMagnitudeTexture` |
| `SpreadTextureOffset` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The uv offset of the `SpreadMagnitudeTexture` |
| `Refract` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this material should also do refraction effects. |
| `RefractionStrength` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | the strength of the refactions |
| `NormalMap` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | The normal map is used as a way to change the appearance of a surface when shined on by lights, to give the illusion of a raised surface. |
| `NormalTextureScale` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The scale of the `NormalMap` texture. |
| `NormalTextureOffset` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The offset of the `NormalMap` texture. |
| `PerObject` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to do the effect per object rather than to the entire image grab pass done by the shader by default. |
| `BlendMode` | **[BlendMode](https://wiki.resonite.com/Type:BlendMode "Type:BlendMode")** | How to blend this material's colors vs what it rendered on top of. |
| `Sidedness` | **[Sidedness](https://wiki.resonite.com/Type:Sidedness "Type:Sidedness")** | Render on both sides of the mesh, front, or back. |
| `ZWrite` | **[ZWrite](https://wiki.resonite.com/Type:ZWrite "Type:ZWrite")** | whether this material should respect the distance it is from the camera. |
| `ZTest` | **[ZTest](https://wiki.resonite.com/Type:ZTest "Type:ZTest")** | Determines whether this object should render when it is in front of or behind other objects that respect depth from the camera |
| `_global` | **[Shader](https://wiki.resonite.com/Type:Shader "Type:Shader")** | [Template:Material global](https://wiki.resonite.com/index.php?title=Template:Material_global&action=edit&redlink=1 "Template:Material global (page does not exist)") |
| `_perObject` | **[Shader](https://wiki.resonite.com/Type:Shader "Type:Shader")** | [Template:Material perObject](https://wiki.resonite.com/index.php?title=Template:Material_perObject&action=edit&redlink=1 "Template:Material perObject (page does not exist)") |

Fields
Collapse

## Usage

Used to make drunk effects, privacy glass, or magic effects.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:BlurMaterial&oldid=105818](https://wiki.resonite.com/index.php?title=Component:BlurMaterial&oldid=105818)"

Contents