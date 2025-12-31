# Component:DebugLinePoint

> Source: https://wiki.resonite.com/Component:DebugLinePoint

Collapse **Component image**

[![](https://wiki.resonite.com/images/7/72/DebugLinePointComponent.png)](https://wiki.resonite.com/File:DebugLinePointComponent.png) **Debug Line Point** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **DebugLinePoint** component draws a line from `LinePoint0` to `LinePoint1` which is the central line. When attached, it generates 128 random Float3's which get added to `Points`. Every point in said list have a line drawn from them to the closest point on the central line.

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This game element is a debug item. Elements like this may be removed at any time without warning, and creations should not rely on it.


## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `LinePoint0` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The starting point of the central line. |
| `LinePoint1` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | the ending point of the central line. |
| `Points` | _direct_ **[SyncFieldList\`1](https://wiki.resonite.com/Type:SyncFieldList%601 "Type:SyncFieldList`1") < [Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3") >** | A list of points to draw lines from to the closest point on the central line. |

Fields
Collapse

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:DebugLinePoint&oldid=96412](https://wiki.resonite.com/index.php?title=Component:DebugLinePoint&oldid=96412)"

Contents