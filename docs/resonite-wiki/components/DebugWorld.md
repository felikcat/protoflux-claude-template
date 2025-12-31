# Component:DebugWorld

> Source: https://wiki.resonite.com/Component:DebugWorld

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/7/73/DebugWorldComponent.png/510px-DebugWorldComponent.png)](https://wiki.resonite.com/File:DebugWorldComponent.png) **Debug World** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **DebugWorld** component renders out a block of text that displays information about the current world the component is in.

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This game element is a debug item. Elements like this may be removed at any time without warning, and creations should not rely on it.


## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `text` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[Sync\`1](https://wiki.resonite.com/Type:Sync%601 "Type:Sync`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | The text field to drive with all the debug data in a world. |

Fields
Collapse

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:DebugWorld&oldid=96400](https://wiki.resonite.com/index.php?title=Component:DebugWorld&oldid=96400)"

Contents