# Component:DebugVector

> Source: https://wiki.resonite.com/Component:DebugVector

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/a/a7/DebugVectorComponent.png/510px-DebugVectorComponent.png)](https://wiki.resonite.com/File:DebugVectorComponent.png) **Debug Vector** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **DebugVector** component shows a vector using a thin line.

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This game element is a debug item. Elements like this may be removed at any time without warning, and creations should not rely on it.


## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `PositionOffset` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | the position offset for the entire Debug visual. |
| `RotationOffset` | **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The rotation Offset for the entire Debug visual. |
| `Vector` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | the vector to debug. |
| `Color` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color of the debug vector line. |
| `UseGlobalSpace` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the vector is in global space or not. |

Fields
Collapse

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:DebugVector&oldid=96384](https://wiki.resonite.com/index.php?title=Component:DebugVector&oldid=96384)"

Contents