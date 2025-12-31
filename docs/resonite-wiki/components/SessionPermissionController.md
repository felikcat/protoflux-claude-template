# Component:SessionPermissionController

> Source: https://wiki.resonite.com/Component:SessionPermissionController

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This is a **[userspace](https://wiki.resonite.com/Userspace "Userspace") component** — you cannot attach it anywhere but the userspace. Messing with the userspace can be fun, but it is **not recommended** as you risk messing your dash up if you don't know what you're doing.


Collapse **Component image**

[File:SessionPermissionControllerComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=SessionPermissionControllerComponent.png "File:SessionPermissionControllerComponent.png") **Session Permission Controller** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **SessionPermissionController** component is used to change the roles or view the roles of a specific user in the current session.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `_name` | **[Text](https://wiki.resonite.com/Component:Text "Component:Text")** | The text element showing the name of the user this belongs to. |
| `_rolesButtons` | _[list](https://wiki.resonite.com/Type:SyncRefList%601 "Type:SyncRefList`1")_ of **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | A list of button elements used to assign the user this belongs to to a role. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| ``SetRole:ButtonEventHandler`1<Int>`` | **[ButtonEventHandler\`1](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler%601&action=edit&redlink=1 "Type:ButtonEventHandler`1 (page does not exist)") < [Int](https://wiki.resonite.com/Type:Int "Type:Int") >** | ✓ | Called when one of the `_rolesButtons` are touched. |

Triggers
Collapse

## Usage

Not to be used directly by the user.

## Examples

Is used in the session tab in the dash.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:SessionPermissionController&oldid=99186](https://wiki.resonite.com/index.php?title=Component:SessionPermissionController&oldid=99186)"

Contents