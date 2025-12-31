# Component:ItemTextureThumbnailSource

> Source: https://wiki.resonite.com/Component:ItemTextureThumbnailSource

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/7/77/ItemTextureThumbnailSourceComponent.png/510px-ItemTextureThumbnailSourceComponent.png)](https://wiki.resonite.com/File:ItemTextureThumbnailSourceComponent.png) **Item Texture Thumbnail Source** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ItemTextureThumbnailSource** component can be used to customize the inventory preview of an item, setting it to a texture.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Texture` | **[Texture2D](https://wiki.resonite.com/Type:Texture2D "Type:Texture2D")** | The texture that should be used as the item's inventory preview. If null, the component will be ignored. |
| `Crop` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Rect](https://wiki.resonite.com/Type:Rect "Type:Rect") >** | The rectangle that defines what section of the image to use. (Or null to use the entire image) |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `OnEnsureSingleThumbnailSource:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | All other components of the same type on the hiearchy of this slot will be deleted when this is pressed. |

Triggers
Collapse

## Usage

To work, the component needs to be attached to the object's root slot and have an image in its `Texture`. The `Ensure single thumbnail source` button can be used to remove all other instances of the component in the item's hierarchy.

## Examples

This component can be used when the automatically generated preview for an item isn't satisfying enough or you want to ensure that the preview looks the same every time or shows the item off in a certain way.

An example of an item that uses this is default Tools in the `Resonite Essentials > Tools` folder.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ItemTextureThumbnailSource&oldid=98604](https://wiki.resonite.com/index.php?title=Component:ItemTextureThumbnailSource&oldid=98604)"

Contents