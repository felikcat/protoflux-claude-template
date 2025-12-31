# Component:InteractiveCameraControlPositioning

> Source: https://wiki.resonite.com/Component:InteractiveCameraControlPositioning

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/4/4f/InteractiveCameraControlPositioningComponent.png/510px-InteractiveCameraControlPositioningComponent.png)](https://wiki.resonite.com/File:InteractiveCameraControlPositioningComponent.png) **Interactive Camera Control Positioning** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

See [Camera](https://wiki.resonite.com/Camera "Camera").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `_canvas` | **[Canvas](https://wiki.resonite.com/Component:Canvas "Component:Canvas")** | The canvas being used to show settings. |
| `_panel` | **[LegacyPanel](https://wiki.resonite.com/Component:LegacyPanel "Component:LegacyPanel")** | The legacy panel being used as a base to interact with the settings. |
| `_control` | **[InteractiveCameraControl](https://wiki.resonite.com/Component:InteractiveCameraControl "Component:InteractiveCameraControl")** | see [Interactive Camera Control](https://wiki.resonite.com/Component:InteractiveCameraControl "Component:InteractiveCameraControl"). |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `OnResetFieldOfView:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | A setting changing handler for the panel. |
| `OnResetAngleOffset:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | A setting changing handler for the panel. |
| `OnResetDistance:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | A setting changing handler for the panel. |
| `OnResetHeight:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | A setting changing handler for the panel. |
| `OnResetFirstPersonPitch:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | A setting changing handler for the panel. |
| `OnResetFirstPersonRoll:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | A setting changing handler for the panel. |
| `OnResetFirstPersonOffset:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | A setting changing handler for the panel. |

Triggers
Collapse

## Usage

See [Camera](https://wiki.resonite.com/Camera "Camera").

## Examples

See [Camera](https://wiki.resonite.com/Camera "Camera").

## See Also

- [Camera](https://wiki.resonite.com/Camera "Camera")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:InteractiveCameraControlPositioning&oldid=98931](https://wiki.resonite.com/index.php?title=Component:InteractiveCameraControlPositioning&oldid=98931)"

Contents