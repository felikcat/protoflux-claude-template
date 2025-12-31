# Component:UserLoginStatus

> Source: https://wiki.resonite.com/Component:UserLoginStatus

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/7/75/UserLoginStatusComponent.png/510px-UserLoginStatusComponent.png)](https://wiki.resonite.com/File:UserLoginStatusComponent.png) **User Login Status** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **UserLoginStatus** component gets the current login status of the local user.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `IsLoggedIn` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the local user is logged in. |
| `LoggedUserId` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | The userID of the local user if they are logged in. |
| `LoggedUsername` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | The username of the local user if they are logged in. |

Fields
Collapse

## Usage

Attach to a Component to instantly get info on the local user's login status.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Component:UserLoginManager](https://wiki.resonite.com/Component:UserLoginManager "Component:UserLoginManager")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:UserLoginStatus&oldid=95830](https://wiki.resonite.com/index.php?title=Component:UserLoginStatus&oldid=95830)"

Contents