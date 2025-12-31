# Component:TiledRawImage

> Source: https://wiki.resonite.com/Component:TiledRawImage

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:TiledRawImage&diff=97783) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/5/57/TiledRawImageComponent.png/510px-TiledRawImageComponent.png)](https://wiki.resonite.com/File:TiledRawImageComponent.png) **TiledRawImage** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **TiledRawImage** component takes in a [ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D") and renders it to the [UIX](https://wiki.resonite.com/UIX "UIX"), and then tiles it if the image provided is too small. There are parameters to control how the tiling behaves for the UIX element that it is in.

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Texture` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | The tilable image to use. |
| `Material` | **[Material](https://wiki.resonite.com/Type:Material "Type:Material")** | The material that has a tilable image to use. |
| `Tint` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The tint color for this image. |
| `SizeBasis` | **[TiledRawImage.TileSizeBasis](https://wiki.resonite.com/Component:TiledRawImage#TileSizeBasis)** | Changes how the tiling behaves. |
| `TileSize` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | How large this image is on the `X` and `Y`. |
| `TileOffset` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | How much this image should be moved on the `X` and `Y`. |
| `InteractionTarget` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Makes this image as the interaction target for this UIX. |

Fields
Collapse

## Usage

This can be used to make fancy backgrounds or image effects. And like with other images, this can be layered for even more effects.

## Examples

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:TiledRawImage&oldid=97783](https://wiki.resonite.com/index.php?title=Component:TiledRawImage&oldid=97783)"

Contents