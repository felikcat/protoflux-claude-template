# Component:InteractiveCameraUserControl

> Source: https://wiki.resonite.com/Component:InteractiveCameraUserControl

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This is a **[userspace](https://wiki.resonite.com/Userspace "Userspace") component** — you cannot attach it anywhere but the userspace. Messing with the userspace can be fun, but it is **not recommended** as you risk messing your dash up if you don't know what you're doing.


Collapse **Component image**

[File:InteractiveCameraUserControlComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=InteractiveCameraUserControlComponent.png "File:InteractiveCameraUserControlComponent.png") **Interactive Camera User Control** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

See [Camera](https://wiki.resonite.com/Camera "Camera").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `_canvas` | **[Canvas](https://wiki.resonite.com/Component:Canvas "Component:Canvas")** | The canvas being used to show settings. |
| `_panel` | **[LegacyPanel](https://wiki.resonite.com/Component:LegacyPanel "Component:LegacyPanel")** | The legacy panel being used as a base to interact with the settings. |
| `Control` | **[InteractiveCameraControl](https://wiki.resonite.com/Component:InteractiveCameraControl "Component:InteractiveCameraControl")** | see [Interactive Camera Control](https://wiki.resonite.com/Component:InteractiveCameraControl "Component:InteractiveCameraControl"). |
| `_uiRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | Where to store UI elements. |

Fields
Collapse

## Usage

See [Camera](https://wiki.resonite.com/Camera "Camera").

## Examples

See [Camera](https://wiki.resonite.com/Camera "Camera").

## See Also

- [Camera](https://wiki.resonite.com/Camera "Camera")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:InteractiveCameraUserControl&oldid=98818](https://wiki.resonite.com/index.php?title=Component:InteractiveCameraUserControl&oldid=98818)"

Contents