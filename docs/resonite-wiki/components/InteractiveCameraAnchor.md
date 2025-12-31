# Component:InteractiveCameraAnchor

> Source: https://wiki.resonite.com/Component:InteractiveCameraAnchor

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/4/40/InteractiveCameraAnchorComponent.png/510px-InteractiveCameraAnchorComponent.png)](https://wiki.resonite.com/File:InteractiveCameraAnchorComponent.png) **Interactive Camera Anchor** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **InteractiveCameraAnchor** component acts as a spot to drop or auto transition a streaming or other type of camera or to.

See [Camera Anchors](https://wiki.resonite.com/Camera#Camera_Anchors "Camera").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `OverrideRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The place other than under this component's slot to parent the cameta. |
| `FieldOfView` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | What the FOV of a camera anchored to this anchor should be set to. |
| `Highlighted` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this anchor is being highlighted as part of specifying a camera anchor set/route. |
| `InUse` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether or not the anchor has a camera in it. |

Fields
Collapse

## Usage

Attaching this component to a slot creates the visual as well as the default values. Simply dropping a stream camera into the visual will snap the camera to it.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

- need a picture of the default anchor with the ghost green model of a camera.

## See Also

- [Component:InteractiveCamera](https://wiki.resonite.com/Component:InteractiveCamera "Component:InteractiveCamera")
- [Camera Anchors](https://wiki.resonite.com/Camera#Camera_Anchors "Camera")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:InteractiveCameraAnchor&oldid=94798](https://wiki.resonite.com/index.php?title=Component:InteractiveCameraAnchor&oldid=94798)"

Contents