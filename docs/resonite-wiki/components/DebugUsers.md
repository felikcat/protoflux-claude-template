# Component:DebugUsers

> Source: https://wiki.resonite.com/Component:DebugUsers

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/a/a4/DebugUsersComponent.png/510px-DebugUsersComponent.png)](https://wiki.resonite.com/File:DebugUsersComponent.png) **Debug Users** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **DebugUsers** component drives get contents of a string field to show statistics of each user in the current world.

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This game element is a debug item. Elements like this may be removed at any time without warning, and creations should not rely on it.


## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `text` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[Sync\`1](https://wiki.resonite.com/Type:Sync%601 "Type:Sync`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | The field to populate with world users statistics. |

Fields
Collapse

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:DebugUsers&oldid=96401](https://wiki.resonite.com/index.php?title=Component:DebugUsers&oldid=96401)"

Contents