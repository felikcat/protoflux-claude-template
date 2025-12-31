# Component:GridTexture

> Source: https://wiki.resonite.com/Component:GridTexture

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:GridTexture&diff=97944) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/1/1c/GridTextureComponent.png/510px-GridTextureComponent.png)](https://wiki.resonite.com/File:GridTextureComponent.png) **Grid Texture** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **GridTexture** component is used to generate a grid of lines with a background color to use in [materials](https://wiki.resonite.com/Materials "Materials").

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
| `BackgroundColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color of the background before `Grids` are layered on top. |
| `Grids` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[GridTexture.Grid](https://wiki.resonite.com/Component:GridTexture#Grid)** | A list of Grids of lines that get layered on top of each other in order. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `BakeTexture:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | BakeTexture first generates a [Component:StaticTexture2D](https://wiki.resonite.com/Component:StaticTexture2D "Component:StaticTexture2D") that is the same as this procedural texture. The resulting static texture replaces every reference to the original procedural texture. Lastly the original procedural texture is deleted. |

Triggers
Collapse

## Grid

| Name | Type | Description |
| --- | --- | --- |
| `Spacing` | **[Int2](https://wiki.resonite.com/Type:Int2 "Type:Int2")** | The distance between lines in pixels for this grid |
| `Offset` | **[Int2](https://wiki.resonite.com/Type:Int2 "Type:Int2")** | The amount to shift this grid around in pixels. can be used to animate movement. |
| `Width` | **[Int2](https://wiki.resonite.com/Type:Int2 "Type:Int2")** | The width of the grid lines in pixels for this grid. |
| `LineColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color of the lines for this grid. |

Fields

## Usage

Attach the component and provide a `BackgroundColor` and add some items to `Grids` to generate the texture. Then add to any [ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D") slot like in [materials](https://wiki.resonite.com/Materials "Materials") for example.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

This needs an example from the default grid world.

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:GridTexture&oldid=97944](https://wiki.resonite.com/index.php?title=Component:GridTexture&oldid=97944)"

Contents