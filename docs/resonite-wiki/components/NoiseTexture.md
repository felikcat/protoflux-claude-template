# Component:NoiseTexture

> Source: https://wiki.resonite.com/Component:NoiseTexture

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:NoiseTexture&diff=98007) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/c/ca/NoiseTextureComponent.png/510px-NoiseTextureComponent.png)](https://wiki.resonite.com/File:NoiseTextureComponent.png) **Noise Texture** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

Noise texture is a component that procedurally generates a 2D texture with a random noise pattern like TV static.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `HighPriorityIntegration` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | If true, integrating this asset (e.g. processing procedural assets) gets higher priority than assets with this flag off. An example is user laser procedural meshes. |
| `FilterMode` | **[TextureFilterMode](https://wiki.resonite.com/Type:TextureFilterMode "Type:TextureFilterMode")** | How to handle the interpolation between pixels. |
| `AnisotropicLevel` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The levels of Anisotropic filtering distances when using Anisotropic for `FilterMode` |
| `WrapModeU` | **[TextureWrapMode](https://wiki.resonite.com/Type:TextureWrapMode "Type:TextureWrapMode")** | How to repeat or mirror the texture along the X axis. this goes into affect when X values are outside of the range \[0.0 to 1.0\]. |
| `WrapModeV` | **[TextureWrapMode](https://wiki.resonite.com/Type:TextureWrapMode "Type:TextureWrapMode")** | How to repeat or mirror the texture along the Y axis. this goes into affect when Y values are outside of the range \[0.0 to 1.0\]. |
| `MipmapBias` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Whether to see lower resolution versions of the texture closer up or not (MipMaps). |
| `Profile` | **[ColorProfile](https://wiki.resonite.com/Type:ColorProfile "Type:ColorProfile")** | The color profile to use for this texture's rendering. |
| `Size` | **[Int2](https://wiki.resonite.com/Type:Int2 "Type:Int2")** | The size of the procedural texture in pixels. |
| `Mipmaps` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to enable the rendering of mipmaps, which are lower res textures at further distances from the camera to improve performance. |
| `Format` | **[TextureFormat](https://wiki.resonite.com/Type:TextureFormat "Type:TextureFormat")** | TextureFormat describes how Texture's pixel are stored in the VRAM. |
| `Seed` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The number to use to seed the generation of the noise for the texture. |
| `Monochrome` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to make the noise generation use a mix of 2 colors rather than random colors. |
| `MonochromeMax` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | Color 1 to use for the noise texture when `Monochrome` is enabled. |
| `MonochromeMin` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | Color 2 to use for the noise texture when `Monochrome` is enabled. |
| `Bias` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The bias to use more of `MonochromeMax` or `MonochromeMin` |
| `Gain` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to brighten the entire texture. |
| `Clamp` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to keep color ranges for the output from going beyond 1 and causing bloom. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `BakeTexture:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | BakeTexture first generates a [Component:StaticTexture2D](https://wiki.resonite.com/Component:StaticTexture2D "Component:StaticTexture2D") that is the same as this procedural texture. The resulting static texture replaces every reference to the original procedural texture. Lastly the original procedural texture is deleted. |

Triggers
Collapse

## Usage

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Can be used as a way of adding texture to surfaces without using an actual stored texture. Can also be used for random TV static on a TV screen.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:NoiseTexture&oldid=98007](https://wiki.resonite.com/index.php?title=Component:NoiseTexture&oldid=98007)"

Contents