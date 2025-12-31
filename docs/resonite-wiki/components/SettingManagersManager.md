# Component:SettingManagersManager

> Source: https://wiki.resonite.com/Component:SettingManagersManager

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This is a **[userspace](https://wiki.resonite.com/Userspace "Userspace") component** — you cannot attach it anywhere but the userspace. Messing with the userspace can be fun, but it is **not recommended** as you risk messing your dash up if you don't know what you're doing.


Collapse **Component image**

[File:SettingManagersManagerComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=SettingManagersManagerComponent.png "File:SettingManagersManagerComponent.png") **Setting Managers Manager** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Setting Managers Manager** component is used to manage the changing from cloud to local setting sets.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `LocalSettings` | **[SettingManager](https://wiki.resonite.com/Component:SettingManager "Component:SettingManager")** | The manager handling locally stored settings. |
| `CloudSettings` | **[SettingManager](https://wiki.resonite.com/Component:SettingManager "Component:SettingManager")** | The manager handling cloud stored settings. |

Fields
Collapse

## See Also

- [Settings](https://wiki.resonite.com/Settings "Settings")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:SettingManagersManager&oldid=100869](https://wiki.resonite.com/index.php?title=Component:SettingManagersManager&oldid=100869)"

Contents