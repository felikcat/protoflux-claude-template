# Component:StaticTexture3D

> Source: https://wiki.resonite.com/Component:StaticTexture3D

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:StaticTexture3D&diff=113607) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/a/a6/StaticTexture3DComponent.png/510px-StaticTexture3DComponent.png)](https://wiki.resonite.com/File:StaticTexture3DComponent.png) **Static Texture 3D** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **StaticTexture3D** component represents a bunch of [textures](https://wiki.resonite.com/Texture2D "Texture2D") stacked on top of each other to make a 3D grid of pixel values, as a [Texture3D](https://wiki.resonite.com/Texture3D "Texture3D"). These textures can be displayed in 3D, or sampled via 3D positions in a few different components or in [ProtoFlux](https://wiki.resonite.com/ProtoFlux "ProtoFlux") Nodes. When [importing a Texture3D](https://wiki.resonite.com/3D_Texture_Import "3D Texture Import"), this component is usually applied after the import.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `URL` | **[Uri](https://wiki.resonite.com/Type:Uri "Type:Uri")** | The address of the texture asset |
| `FilterMode` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [TextureFilterMode](https://wiki.resonite.com/Type:TextureFilterMode "Type:TextureFilterMode") >** | How to handle the interpolation between pixels. |
| `AnisotropicLevel` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Int](https://wiki.resonite.com/Type:Int "Type:Int") >** | The levels of Anisotropic filtering distances when using Anisotropic for `FilterMode` |
| `Uncompressed` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to not compress the texture's size before loading into ram/vram. doesn't affect cloud size. |
| `DirectLoad` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to not cache the texture in the local cache for [Resonite](https://wiki.resonite.com/Resonite "Resonite") |
| `ForceExactVariant` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to not generate variants for this texture and force a certain texture type |
| `PreferredFormat` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [TextureCompression](https://wiki.resonite.com/Type:TextureCompression "Type:TextureCompression") >** | The format to use for texture compression rather than the auto picked one |
| `PreferredProfile` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [ColorProfile](https://wiki.resonite.com/Type:ColorProfile "Type:ColorProfile") >** | The color profile to use rather than the auto picked one. (usually linear) |
| `MipMapBias` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Whether to see lower resolution versions of the texture closer up or not (MipMaps). |
| `WrapModeU` | **[TextureWrapMode](https://wiki.resonite.com/Type:TextureWrapMode "Type:TextureWrapMode")** | How to repeat or mirror the texture along the X axis. this goes into affect when X values are outside of the range \[0.0 to 1.0\]. |
| `WrapModeV` | **[TextureWrapMode](https://wiki.resonite.com/Type:TextureWrapMode "Type:TextureWrapMode")** | How to repeat or mirror the texture along the Y axis. this goes into affect when Y values are outside of the range \[0.0 to 1.0\]. |
| `WrapModeW` | **[TextureWrapMode](https://wiki.resonite.com/Type:TextureWrapMode "Type:TextureWrapMode")** | How to repeat or mirror the texture along the Z axis. this goes into affect when Z values are outside of the range \[0.0 to 1.0\]. |
| `Readable` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether or not the texture can be sampled via texture sampling ProtoFlux nodes |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| ``InvertRGB:Func`1<Task`1<Bool>>`` | **[Func\`1](https://wiki.resonite.com/Type:Func%601 "Type:Func`1") < [Task\`1](https://wiki.resonite.com/index.php?title=Type:Task%601&action=edit&redlink=1 "Type:Task`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >>** | X | Inverts the colors of the image. |
| ``InvertR:Func`1<Task`1<Bool>>`` | **[Func\`1](https://wiki.resonite.com/Type:Func%601 "Type:Func`1") < [Task\`1](https://wiki.resonite.com/index.php?title=Type:Task%601&action=edit&redlink=1 "Type:Task`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >>** | X | Inverts the red channel of the image. |
| ``InvertG:Func`1<Task`1<Bool>>`` | **[Func\`1](https://wiki.resonite.com/Type:Func%601 "Type:Func`1") < [Task\`1](https://wiki.resonite.com/index.php?title=Type:Task%601&action=edit&redlink=1 "Type:Task`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >>** | X | Inverts the green channel of the image. |
| ``InvertB:Func`1<Task`1<Bool>>`` | **[Func\`1](https://wiki.resonite.com/Type:Func%601 "Type:Func`1") < [Task\`1](https://wiki.resonite.com/index.php?title=Type:Task%601&action=edit&redlink=1 "Type:Task`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >>** | X | Inverts the blue channel of the image. |
| ``InvertA:Func`1<Task`1<Bool>>`` | **[Func\`1](https://wiki.resonite.com/Type:Func%601 "Type:Func`1") < [Task\`1](https://wiki.resonite.com/index.php?title=Type:Task%601&action=edit&redlink=1 "Type:Task`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >>** | X | Inverts the alpha channel of the image. |
| ``ColorToAlpha:Func`2<ColorX, Task`1<Bool>>`` | **[Func\`2](https://wiki.resonite.com/Type:Func%602 "Type:Func`2") < [ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX"), [Task\`1](https://wiki.resonite.com/index.php?title=Type:Task%601&action=edit&redlink=1 "Type:Task`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >>** | X | Turns the color data of the image into transparency/alpha data. |
| ``AlphaFromIntensity:Func`1<Task`1<Bool>>`` | **[Func\`1](https://wiki.resonite.com/Type:Func%601 "Type:Func`1") < [Task\`1](https://wiki.resonite.com/index.php?title=Type:Task%601&action=edit&redlink=1 "Type:Task`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >>** | X | Makes alpha/transparency data depending on the color intensity of the image. |
| ``AlphaToMask:Func`1<Task`1<Bool>>`` | **[Func\`1](https://wiki.resonite.com/Type:Func%601 "Type:Func`1") < [Task\`1](https://wiki.resonite.com/index.php?title=Type:Task%601&action=edit&redlink=1 "Type:Task`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >>** | X | Turns the alpha of the image into a black and white image. |
| ``RemoveAlpha:Func`1<Task`1<Bool>>`` | **[Func\`1](https://wiki.resonite.com/Type:Func%601 "Type:Func`1") < [Task\`1](https://wiki.resonite.com/index.php?title=Type:Task%601&action=edit&redlink=1 "Type:Task`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >>** | X | Removes the alpha data completely from the image or makes it white. |
| ``GrayscaleAverage:Func`1<Task`1<Bool>>`` | **[Func\`1](https://wiki.resonite.com/Type:Func%601 "Type:Func`1") < [Task\`1](https://wiki.resonite.com/index.php?title=Type:Task%601&action=edit&redlink=1 "Type:Task`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >>** | X | Make grayscale image based on the average values for the colors per pixel. |
| ``GrayscaleLuminance:Func`1<Task`1<Bool>>`` | **[Func\`1](https://wiki.resonite.com/Type:Func%601 "Type:Func`1") < [Task\`1](https://wiki.resonite.com/index.php?title=Type:Task%601&action=edit&redlink=1 "Type:Task`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >>** | X | Make grayscale image based on the color luminance per pixel. |
| ``SwapRG:Func`1<Task`1<Bool>>`` | **[Func\`1](https://wiki.resonite.com/Type:Func%601 "Type:Func`1") < [Task\`1](https://wiki.resonite.com/index.php?title=Type:Task%601&action=edit&redlink=1 "Type:Task`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >>** | X | Swaps the red and green channels on the image |
| ``SwapRB:Func`1<Task`1<Bool>>`` | **[Func\`1](https://wiki.resonite.com/Type:Func%601 "Type:Func`1") < [Task\`1](https://wiki.resonite.com/index.php?title=Type:Task%601&action=edit&redlink=1 "Type:Task`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >>** | X | Swaps the red and blue channels on the image |
| ``SwapRA:Func`1<Task`1<Bool>>`` | **[Func\`1](https://wiki.resonite.com/Type:Func%601 "Type:Func`1") < [Task\`1](https://wiki.resonite.com/index.php?title=Type:Task%601&action=edit&redlink=1 "Type:Task`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >>** | X | Swaps the red and alpha channels on the image |
| ``SwapGB:Func`1<Task`1<Bool>>`` | **[Func\`1](https://wiki.resonite.com/Type:Func%601 "Type:Func`1") < [Task\`1](https://wiki.resonite.com/index.php?title=Type:Task%601&action=edit&redlink=1 "Type:Task`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >>** | X | Swaps the green and blue channels on the image |
| ``SwapGA:Func`1<Task`1<Bool>>`` | **[Func\`1](https://wiki.resonite.com/Type:Func%601 "Type:Func`1") < [Task\`1](https://wiki.resonite.com/index.php?title=Type:Task%601&action=edit&redlink=1 "Type:Task`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >>** | X | Swaps the green and alpha channels on the image |
| ``SwapBA:Func`1<Task`1<Bool>>`` | **[Func\`1](https://wiki.resonite.com/Type:Func%601 "Type:Func`1") < [Task\`1](https://wiki.resonite.com/index.php?title=Type:Task%601&action=edit&redlink=1 "Type:Task`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >>** | X | Swaps the blue and alpha channels on the image |
| ``AddBackground:Func`2<ColorX, Task`1<Bool>>`` | **[Func\`2](https://wiki.resonite.com/Type:Func%602 "Type:Func`2") < [ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX"), [Task\`1](https://wiki.resonite.com/index.php?title=Type:Task%601&action=edit&redlink=1 "Type:Task`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >>** | X | adds a background of a color to a transparent image. |
| ``AdjustGamma:Func`2<Float, Task`1<Bool>>`` | **[Func\`2](https://wiki.resonite.com/Type:Func%602 "Type:Func`2") < [Float](https://wiki.resonite.com/Type:Float "Type:Float"), [Task\`1](https://wiki.resonite.com/index.php?title=Type:Task%601&action=edit&redlink=1 "Type:Task`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >>** | X | Adjusts the gamma of the image. |
| ``AdjustAlphaGamma:Func`2<Float, Task`1<Bool>>`` | **[Func\`2](https://wiki.resonite.com/Type:Func%602 "Type:Func`2") < [Float](https://wiki.resonite.com/Type:Float "Type:Float"), [Task\`1](https://wiki.resonite.com/index.php?title=Type:Task%601&action=edit&redlink=1 "Type:Task`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >>** | X | Adjusts the gamma of the alpha channel of the image. |
| ``ShiftHue:Func`2<Float, Task`1<Bool>>`` | **[Func\`2](https://wiki.resonite.com/Type:Func%602 "Type:Func`2") < [Float](https://wiki.resonite.com/Type:Float "Type:Float"), [Task\`1](https://wiki.resonite.com/index.php?title=Type:Task%601&action=edit&redlink=1 "Type:Task`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >>** | X | Shifts the hue of HSV of the image. |
| ``SetHue:Func`2<Float, Task`1<Bool>>`` | **[Func\`2](https://wiki.resonite.com/Type:Func%602 "Type:Func`2") < [Float](https://wiki.resonite.com/Type:Float "Type:Float"), [Task\`1](https://wiki.resonite.com/index.php?title=Type:Task%601&action=edit&redlink=1 "Type:Task`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >>** | X | Sets the Hue of HSV of the image. |
| ``SetSaturation:Func`2<Float, Task`1<Bool>>`` | **[Func\`2](https://wiki.resonite.com/Type:Func%602 "Type:Func`2") < [Float](https://wiki.resonite.com/Type:Float "Type:Float"), [Task\`1](https://wiki.resonite.com/index.php?title=Type:Task%601&action=edit&redlink=1 "Type:Task`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >>** | X | Sets the saturation of HSV of the image. |
| ``OffsetSaturation:Func`2<Float, Task`1<Bool>>`` | **[Func\`2](https://wiki.resonite.com/Type:Func%602 "Type:Func`2") < [Float](https://wiki.resonite.com/Type:Float "Type:Float"), [Task\`1](https://wiki.resonite.com/index.php?title=Type:Task%601&action=edit&redlink=1 "Type:Task`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >>** | X | Adds to the saturation of HSV of the image. |
| ``MulSaturation:Func`2<Float, Task`1<Bool>>`` | **[Func\`2](https://wiki.resonite.com/Type:Func%602 "Type:Func`2") < [Float](https://wiki.resonite.com/Type:Float "Type:Float"), [Task\`1](https://wiki.resonite.com/index.php?title=Type:Task%601&action=edit&redlink=1 "Type:Task`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >>** | X | Multiplies the saturation of HSV of the image. |
| ``SetValue:Func`2<Float, Task`1<Bool>>`` | **[Func\`2](https://wiki.resonite.com/Type:Func%602 "Type:Func`2") < [Float](https://wiki.resonite.com/Type:Float "Type:Float"), [Task\`1](https://wiki.resonite.com/index.php?title=Type:Task%601&action=edit&redlink=1 "Type:Task`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >>** | X | Sets the value of HSV of the image. |
| ``MulValue:Func`2<Float, Task`1<Bool>>`` | **[Func\`2](https://wiki.resonite.com/Type:Func%602 "Type:Func`2") < [Float](https://wiki.resonite.com/Type:Float "Type:Float"), [Task\`1](https://wiki.resonite.com/index.php?title=Type:Task%601&action=edit&redlink=1 "Type:Task`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >>** | X | Multiplies the value of HSV of the image. |
| ``OffsetValue:Func`2<Float, Task`1<Bool>>`` | **[Func\`2](https://wiki.resonite.com/Type:Func%602 "Type:Func`2") < [Float](https://wiki.resonite.com/Type:Float "Type:Float"), [Task\`1](https://wiki.resonite.com/index.php?title=Type:Task%601&action=edit&redlink=1 "Type:Task`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >>** | X | Adds to the value of HSV of the image. |
| ``OffsetAlpha:Func`2<Float, Task`1<Bool>>`` | **[Func\`2](https://wiki.resonite.com/Type:Func%602 "Type:Func`2") < [Float](https://wiki.resonite.com/Type:Float "Type:Float"), [Task\`1](https://wiki.resonite.com/index.php?title=Type:Task%601&action=edit&redlink=1 "Type:Task`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >>** | X | Adds to the alpha of the image. |
| ``Normalize:Func`4<Bool, Bool, Bool, Task`1<Bool>>`` | **[Func\`4](https://wiki.resonite.com/Type:Func%604 "Type:Func`4") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool"), [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool"), [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool"), [Task\`1](https://wiki.resonite.com/index.php?title=Type:Task%601&action=edit&redlink=1 "Type:Task`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >>** | X | Normalizes the colors of the image, making it have a bigger color range usage. |

Triggers
Collapse

## Usage

Is generated automatically when importing a folder of images that are slices of a cube stacked vertically. Insert into a [Component:VolumeUnlitMaterial](https://wiki.resonite.com/Component:VolumeUnlitMaterial "Component:VolumeUnlitMaterial") to view the colors or a [Component:LUT Material](https://wiki.resonite.com/Component:LUT_Material "Component:LUT Material") to view it's affect as a filter.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:StaticTexture3D&oldid=113607](https://wiki.resonite.com/index.php?title=Component:StaticTexture3D&oldid=113607)"

Contents