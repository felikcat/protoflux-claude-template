# Component:AudioInputDeviceSettings

> Source: https://wiki.resonite.com/Component:AudioInputDeviceSettings

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/5/50/AudioInputDeviceSettingsComponent.png/510px-AudioInputDeviceSettingsComponent.png)](https://wiki.resonite.com/File:AudioInputDeviceSettingsComponent.png) **Audio Input Device Settings** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **AudioInputDeviceSettings** Component is used to set the priority order of input devices for the local user. It also can be used to disable priority and use the system default instead.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `UseSystemDefault` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether or not to use the user's default device on their OS or not. |
| `DevicePriorities` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[DevicePriorityEntry](https://wiki.resonite.com/Type:DevicePriorityEntry "Type:DevicePriorityEntry")** | A list of devices and their priority which is the order to use them in. |
| `DevicePrioritiesEnabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the "Use Default Device" setting is turned on or off |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `GetDevice:SubsettingGetter` | **[SubsettingGetter](https://wiki.resonite.com/Type:SubsettingGetter "Type:SubsettingGetter")** | X | This returns a setting with the name specified by the methods `key` input. |

Triggers
Collapse

## Usage

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Examples

The settings menu

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AudioInputDeviceSettings&oldid=99152](https://wiki.resonite.com/index.php?title=Component:AudioInputDeviceSettings&oldid=99152)"

Contents