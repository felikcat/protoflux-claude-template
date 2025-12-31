# Component:WorldCaptureThumbnailSource

> Source: https://wiki.resonite.com/Component:WorldCaptureThumbnailSource

Collapse **Component image**

[File:WorldCaptureThumbnailSourceComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=WorldCaptureThumbnailSourceComponent.png "File:WorldCaptureThumbnailSourceComponent.png") **World Capture Thumbnail Source** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **WorldCaptureThumbnailSource** component is used as a point in space to capture the preview of a world in the world browser minus users in the session when a world is saved.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Overlay` | **[Texture2D](https://wiki.resonite.com/Type:Texture2D "Type:Texture2D")** | The texture to use as an overlay for capturing the thumbnail. |
| `ExcludeUsersInCapture` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to exclude users from the thumbnail. |

Fields
Collapse

## Usage

see: [World and Session Thumbnails#Customising Thumbnails](https://wiki.resonite.com/World_and_Session_Thumbnails#Customising_Thumbnails "World and Session Thumbnails")

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Component:SessionCaptureThumbnailSource](https://wiki.resonite.com/Component:SessionCaptureThumbnailSource "Component:SessionCaptureThumbnailSource") for capturing the session preview for a particular world instance.

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:WorldCaptureThumbnailSource&oldid=100820](https://wiki.resonite.com/index.php?title=Component:WorldCaptureThumbnailSource&oldid=100820)"

Contents