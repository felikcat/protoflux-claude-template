# Component:RawImage

> Source: https://wiki.resonite.com/Component:RawImage

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:RawImage&diff=88637) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/b/b2/RawImageComponent.png/510px-RawImageComponent.png)](https://wiki.resonite.com/File:RawImageComponent.png) **RawImage** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **RawImage** component takes in a [ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D") and takes in parameters to alter this texture image.

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Texture` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | The texture image itself. |
| `Material` | **[Material](https://wiki.resonite.com/Type:Material "Type:Material")** | The material to use as the texture from. |
| `Tint` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The tint color for this raw image. |
| `UVRect` | **[Rect](https://wiki.resonite.com/Type:Rect "Type:Rect")** | Shifts the UV of the raw image. |
| `Orientation` | **[RectOrientation](https://wiki.resonite.com/index.php?title=Type:RectOrientation&action=edit&redlink=1 "Type:RectOrientation (page does not exist)")** | Rotates the raw image and respects aspect ratio. |
| `PreserveAspect` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | If this raw graphic should preserve its aspect ratio. |
| `InteractionTarget` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Makes this image as the interaction target for this UIX. |

Fields
Collapse

## Usage

This component acts more like a holder for a texture image to be used by other components.

## Examples

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:RawImage&oldid=88637](https://wiki.resonite.com/index.php?title=Component:RawImage&oldid=88637)"

Contents