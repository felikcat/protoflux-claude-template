# Component:UserLoginManager

> Source: https://wiki.resonite.com/Component:UserLoginManager

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/3/31/UserLoginManagerComponent.png/510px-UserLoginManagerComponent.png)](https://wiki.resonite.com/File:UserLoginManagerComponent.png) **UserLoginManager** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **UserLoginManager** component is used to handle the user's login status.

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `IsLoggedIn` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the current user is logged in or not. |
| `IsLoggingOut` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the local user is currently logging out or not. |
| `CurrentUsername` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | The username of the local user. |
| `CurrentUserId` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | The user ID of the local user. |
| `CurrentAccountType` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | The account type of the local user (patreon status or team member likewise) |
| `CurrentAccountColorOverride` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX") >** | The current user color override of the local user. Like nametag colors. |
| `CurrentProfileIcon` | **[Uri](https://wiki.resonite.com/Type:Uri "Type:Uri")** | The user icon of the local user. |
| `LoginLogoutButton` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | Only works in [userspace](https://wiki.resonite.com/Userspace "Userspace"). Is the button for logging in or out. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `DoLoginLogout:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | X | Triggers the login/logout process. |

Triggers
Collapse

## Usage

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Examples

The UserProfile facet in [Resonite Essentials](https://wiki.resonite.com/Resonite_Essentials "Resonite Essentials") uses UserLoginManager for getting profile information and logging out the user:

- `resrec:///G-Resonite/R-c01a8b5b-be64-4b35-aa16-a20ff5f8a030`

## See Also

- [Dash Menu](https://wiki.resonite.com/Dash_Menu "Dash Menu")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:UserLoginManager&oldid=100796](https://wiki.resonite.com/index.php?title=Component:UserLoginManager&oldid=100796)"

Contents