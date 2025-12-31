# Component:UserInfo

> Source: https://wiki.resonite.com/Component:UserInfo

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:UserInfo&diff=95825) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/4/46/UserInfoComponent.png/510px-UserInfoComponent.png)](https://wiki.resonite.com/File:UserInfoComponent.png) **User Info** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **UserInfo** component handles keeping certain bits of data about a player spawned physically in the world. It's stored under the user root slot.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Controllers` | _[list](https://wiki.resonite.com/Type:SyncRefList%601 "Type:SyncRefList`1")_ of **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slots of the controllers this user is using. |
| `Hands` | _[list](https://wiki.resonite.com/Type:SyncRefList%601 "Type:SyncRefList`1")_ of **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slots of the hands this user. |

Fields
Collapse

## Usage

Used internally.

## Examples

Seen in the root of a user root of a player.

## See Also

- [Component:UserRoot](https://wiki.resonite.com/Component:UserRoot "Component:UserRoot")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:UserInfo&oldid=95825](https://wiki.resonite.com/index.php?title=Component:UserInfo&oldid=95825)"

Contents