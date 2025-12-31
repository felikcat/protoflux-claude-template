# Component:GrayscaleMaterial

> Source: https://wiki.resonite.com/Component:GrayscaleMaterial

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:GrayscaleMaterial&diff=105830) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/e/e0/GrayscaleMaterialComponent.png/510px-GrayscaleMaterialComponent.png)](https://wiki.resonite.com/File:GrayscaleMaterialComponent.png) **GrayscaleMaterial** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **GrayscaleMaterial** component is a material that allows the mapping of grayscale values from 0 to 1 to any other value. This is analogous to the [Color Ramp](https://docs.blender.org/manual/en/latest/render/shader_nodes/converter/color_ramp.html) node in Blender. A common misconception is that this can only produce black and white values, however that is only the default gradient, and a user-provided **Gradient** texture allows for various colored effects.

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
| `RatioRed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The proportion of red to use for grayscale computation |
| `RatioGreen` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The proportion of green to use for grayscale computation |
| `RatioBlue` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The proportion of blue to use for grayscale computation |
| `Lerp` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The value to use to transition between the first and second texture and value sets in absence of `LerpTexture`. |
| `Gradient` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | A texture which maps black values on its far left and white values on its far right |
| `BlendMode` | **[BlendMode](https://wiki.resonite.com/Type:BlendMode "Type:BlendMode")** | How to blend this material's colors vs what it rendered on top of. |
| `Sidedness` | **[Sidedness](https://wiki.resonite.com/Type:Sidedness "Type:Sidedness")** | Render on both sides of the mesh, front, or back. |
| `ZWrite` | **[ZWrite](https://wiki.resonite.com/Type:ZWrite "Type:ZWrite")** | whether this material should respect the distance it is from the camera. |
| `ZTest` | **[ZTest](https://wiki.resonite.com/Type:ZTest "Type:ZTest")** | Determines whether this object should render when it is in front of or behind other objects that respect depth from the camera |

Fields
Collapse

## Behavior

This material acts as a filter which applies on top of other materials.

It first computes a grayscale value for all pixels that overlap with the filter which is computed through a weighted combination of Red, Green, and Blue values that can be directly controlled through the respective ratio inputs.

A user-provided **Gradient** texture defines how these values are then remapped. The leftmost part of this texture defines what color will correspond to Black (0) and the rightmost part of this texture defines the color that maps to White (1). It is important to set the [WrapModeU](https://wiki.resonite.com/index.php?title=WrapModeU&action=edit&redlink=1 "WrapModeU (page does not exist)") of this texture to **Clamp** or else it will bleed values from either side of the texture.

The **Lerp** field allows you to transition between having the filter off (0) and fully on (1).

## Examples

[![Grayscale Filter Lerp 0](https://wiki.resonite.com/images/thumb/c/c0/GrayscaleMaterial_lerp0.webp/800px-GrayscaleMaterial_lerp0.webp.png)](https://wiki.resonite.com/File:GrayscaleMaterial_lerp0.webp) Without GrayscaleMaterial applied[![Grayscale Filter Default](https://wiki.resonite.com/images/thumb/4/44/GrayscaleMaterial_lerp1_default.webp/800px-GrayscaleMaterial_lerp1_default.webp.png)](https://wiki.resonite.com/File:GrayscaleMaterial_lerp1_default.webp) Default GrayscaleMaterial[![Rainbow Grayscale Filter](https://wiki.resonite.com/images/thumb/4/42/GrayscaleMaterial_rainbow.webp/800px-GrayscaleMaterial_rainbow.webp.png)](https://wiki.resonite.com/File:GrayscaleMaterial_rainbow.webp) GrayscaleMaterial with a rainbow Gradient texture

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:GrayscaleMaterial&oldid=105830](https://wiki.resonite.com/index.php?title=Component:GrayscaleMaterial&oldid=105830)"

Contents