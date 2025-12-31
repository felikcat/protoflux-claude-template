# Component:UserspaceScreensManager

> Source: https://wiki.resonite.com/Component:UserspaceScreensManager

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This is a **[userspace](https://wiki.resonite.com/Userspace "Userspace") component** — you cannot attach it anywhere but the userspace. Messing with the userspace can be fun, but it is **not recommended** as you risk messing your dash up if you don't know what you're doing.


Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/8/87/UserspaceScreensManagerComponent.png/510px-UserspaceScreensManagerComponent.png)](https://wiki.resonite.com/File:UserspaceScreensManagerComponent.png) **Userspace Screens Manager** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **UserspaceScreensManager** component is used in the user space and handles login status and unread notifications.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `_loginStatus` | **[UserLoginStatus](https://wiki.resonite.com/Component:UserLoginStatus "Component:UserLoginStatus")** | The current login status of the user. |
| `_unreadIndicator` | **[Text](https://wiki.resonite.com/Component:Text "Component:Text")** | How many unread notifications the user has, which is driven to the specified text element. |

Fields
Collapse

## Usage

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:UserspaceScreensManager&oldid=106615](https://wiki.resonite.com/index.php?title=Component:UserspaceScreensManager&oldid=106615)"

Contents