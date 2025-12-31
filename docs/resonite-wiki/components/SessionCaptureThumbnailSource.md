# Component:SessionCaptureThumbnailSource

> Source: https://wiki.resonite.com/Component:SessionCaptureThumbnailSource

Collapse **Component image**

[File:SessionCaptureThumbnailSourceComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=SessionCaptureThumbnailSourceComponent.png "File:SessionCaptureThumbnailSourceComponent.png") **Session Capture Thumbnail Source** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **SessionCaptureThumbnailSource** component sets the slot it is on as a source for capturing the [session thumbnail](https://wiki.resonite.com/Session_thumbnail "Session thumbnail"), or the preview image used for the currently active session.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Overlay` | **[Texture2D](https://wiki.resonite.com/Type:Texture2D "Type:Texture2D")** | An overlay image to superimpose over the normal session capture. This image must have an average alpha channel value under 25% or else it will not be applied. |

Fields
Collapse

## Usage

Place this component on a slot. The slot's position will then be used as the capture source for the [session thumbnail](https://wiki.resonite.com/Session_thumbnail "Session thumbnail"). If multiple slots have this component on it, the capture will be taken via a weighted random pick, where slots with a lower average user distance from them will be more likely to be captured.

## See also

- [Component:WorldCaptureThumbnailSource](https://wiki.resonite.com/Component:WorldCaptureThumbnailSource "Component:WorldCaptureThumbnailSource") for capturing the world preview that shows up without an active session.

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:SessionCaptureThumbnailSource&oldid=104370](https://wiki.resonite.com/index.php?title=Component:SessionCaptureThumbnailSource&oldid=104370)"

Contents