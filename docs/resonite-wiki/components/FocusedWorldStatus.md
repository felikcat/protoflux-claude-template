# Component:FocusedWorldStatus

> Source: https://wiki.resonite.com/Component:FocusedWorldStatus

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:FocusedWorldStatus&diff=113233) which are not marked for translation.

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This is a **[userspace](https://wiki.resonite.com/Userspace "Userspace") component** — you cannot attach it anywhere but the userspace. Messing with the userspace can be fun, but it is **not recommended** as you risk messing your dash up if you don't know what you're doing.


Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/3/3a/FocusedWorldStatusComponent.png/510px-FocusedWorldStatusComponent.png)](https://wiki.resonite.com/File:FocusedWorldStatusComponent.png) **Focused World Status** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

**FocusedWorldStatus** is a component that displays information about the currently focused world. It's used in the session tab in the [dash](https://wiki.resonite.com/Dash "Dash").

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `WorldName` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The name of the currently focused world. |
| `RawWorldName` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The raw unfiltered name of the currently focused world. |
| `SessionId` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The session ID of the currently focused world. |
| `IsHost` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the user is the host of the focused world. |
| `CanSave` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the user is allowed to save the focused world. |
| `ShouldSave` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the focused world has unsaved changes or not. |
| `CanClose` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the focused world can be closed. False for the [Local Home](https://wiki.resonite.com/Local_Home "Local Home"). |
| `RoleName` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The name of the role that the user currently has in the focused world. |
| `UserCount` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The amount of users currently in the focused world. |
| `ActiveUserCount` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | How many of the users in the focused world aren't AFK. |
| `MaxUserCount` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The maximum amount of users that can be in the focused world. |
| `AccessLevel` | **[SessionAccessLevel](https://wiki.resonite.com/Type:SessionAccessLevel "Type:SessionAccessLevel")** | The access level of the focused world. |
| `HideFromListing` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether or not the focused world should not be shown in world listings or shown to other users. |
| `AwayKickEnabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the focused world has AFK kick enabled. |
| `AwayKickMinutes` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How many minutes a user can be AFK before being kicked from the focused world. |
| `UnsafeMode` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the focused world is in [unsafe mode](https://wiki.resonite.com/index.php?title=Unsafe_mode&action=edit&redlink=1 "Unsafe mode (page does not exist)"), which allows for some features to work. Can only be true in private worlds. |

Fields
Collapse

## Usage

Used in the dash, and isn't utilizable in normal gameplay.

## Examples

Used in the dash.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:FocusedWorldStatus&oldid=113233](https://wiki.resonite.com/index.php?title=Component:FocusedWorldStatus&oldid=113233)"

Contents