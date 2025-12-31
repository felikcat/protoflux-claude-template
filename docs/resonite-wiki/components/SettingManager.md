# Component:SettingManager

> Source: https://wiki.resonite.com/Component:SettingManager

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This is a **[userspace](https://wiki.resonite.com/Userspace "Userspace") component** — you cannot attach it anywhere but the userspace. Messing with the userspace can be fun, but it is **not recommended** as you risk messing your dash up if you don't know what you're doing.


Collapse **Component image**

[File:SettingManagerComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=SettingManagerComponent.png "File:SettingManagerComponent.png") **Setting Manager** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Setting Manager** component is internally used by the settings system to handle settings changes.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `OwnerId` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The owner of the settings that this manages. |
| `SupressedBy` | **SettingManager** | Whether changes in this are suppressed by another setting manager. |

Fields
Collapse

## Usage

See [Settings](https://wiki.resonite.com/Settings "Settings").

## Examples

See [Settings](https://wiki.resonite.com/Settings "Settings").

## See Also

- [Settings](https://wiki.resonite.com/Settings "Settings")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:SettingManager&oldid=100865](https://wiki.resonite.com/index.php?title=Component:SettingManager&oldid=100865)"

Contents