# Component:LUT Material

> Source: https://wiki.resonite.com/Component:LUT_Material

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:LUT_Material&diff=113618) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/6/62/LUT_MaterialComponent.png/510px-LUT_MaterialComponent.png)](https://wiki.resonite.com/File:LUT_MaterialComponent.png) **LUT Material** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

A [LUT (Lookup Table)](https://en.wikipedia.org/wiki/Lookup_table) is a way of mapping input values to output values via sampling a [Texture3D](https://wiki.resonite.com/Texture3D "Texture3D") with the [StaticTexture3D](https://wiki.resonite.com/Component:StaticTexture3D "Component:StaticTexture3D") component. This 3D table of values allows for any arbitrary function to be applied to an input.

How the sampling works is that it takes a color behind it (for example, a magenta color) and maps it's RGB values to a 0-1 [Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3") as XYZ, it then samples the provided 3D texture at point XYZ multiplied by the texture's size, and uses the pixel's color as the result which is applied to what the user sees through this material.

For more info on how pixels are arranged on a 3D texture and can be retrieved using an [Int3](https://wiki.resonite.com/Type:Int3 "Type:Int3"), see [3D Texture Import](https://wiki.resonite.com/3D_Texture_Import "3D Texture Import").

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
| `LUT` | **[Texture3D](https://wiki.resonite.com/Type:Texture3D "Type:Texture3D")** | The [3D texture](https://wiki.resonite.com/Texture3D "Texture3D") to use as a lookup table |
| `SecondaryLUT` | **[Texture3D](https://wiki.resonite.com/Type:Texture3D "Type:Texture3D")** | A secondary 3D texture to use to lerp between |
| `UseSRGB` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to use the SRGB color space when spitting out colors. |
| `Lerp` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The value to use to transition between the first and second texture and value sets in absence of `LerpTexture`. |
| `BlendMode` | **[BlendMode](https://wiki.resonite.com/Type:BlendMode "Type:BlendMode")** | How to blend this material's colors vs what it rendered on top of. |
| `Sidedness` | **[Sidedness](https://wiki.resonite.com/Type:Sidedness "Type:Sidedness")** | Render on both sides of the mesh, front, or back. |
| `ZWrite` | **[ZWrite](https://wiki.resonite.com/Type:ZWrite "Type:ZWrite")** | whether this material should respect the distance it is from the camera. |
| `ZTest` | **[ZTest](https://wiki.resonite.com/Type:ZTest "Type:ZTest")** | Determines whether this object should render when it is in front of or behind other objects that respect depth from the camera |

Fields
Collapse

## Usage

The mapping function of an LUT takes an input RGB value and then samples the 3D Texture at that corresponding coordinate to find the output RGB value, using the [3D Texture](https://wiki.resonite.com/StaticTexture3D_(Component) "StaticTexture3D (Component)")'s [Filter Mode](https://wiki.resonite.com/Type:TextureFilterMode "Type:TextureFilterMode") and [Wrap Mode](https://wiki.resonite.com/Type:TextureWrapMode "Type:TextureWrapMode") to resolve how intermediate values work.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

We need (an image of a scene behind a plane as well as the cube of the 3d texture being used):

- an example of an LUT material making a Gameboy effect of materials behind it
- an example of an LUT making a grayscale effect of materials behind it
- an example of an LUT that inverts materials behind it
- an example of an LUT that makes materials behind it that have shades of red in their surface spit out random nonsensical colors depending on brightness (yes this is possible with an LUT)

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:LUT\_Material&oldid=113618](https://wiki.resonite.com/index.php?title=Component:LUT_Material&oldid=113618)"

Contents