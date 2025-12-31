# Component:DebugTransform

> Source: https://wiki.resonite.com/Component:DebugTransform

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/2/21/DebugTransformComponent.png/510px-DebugTransformComponent.png)](https://wiki.resonite.com/File:DebugTransformComponent.png) **Debug Transform** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **DebugTransform** component is used to show the parent hiearchy of a slot in the form of text to a specific `ShowToUser`.

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This game element is a debug item. Elements like this may be removed at any time without warning, and creations should not rely on it.


## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `ShowToUser` | _direct_ **[UserRef](https://wiki.resonite.com/Type:UserRef "Type:UserRef")** | Shows the debug visual to this user only. |

Fields
Collapse

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:DebugTransform&oldid=96386](https://wiki.resonite.com/index.php?title=Component:DebugTransform&oldid=96386)"

Contents