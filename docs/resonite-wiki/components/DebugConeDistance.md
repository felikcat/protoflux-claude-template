# Component:DebugConeDistance

> Source: https://wiki.resonite.com/Component:DebugConeDistance

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/8/8f/DebugConeDistanceComponent.png/510px-DebugConeDistanceComponent.png)](https://wiki.resonite.com/File:DebugConeDistanceComponent.png) **Debug Cone Distance** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **DebugConeDistance** component creates a Debug cone visual that draws lines from the list of `Points` to the surface of the cone. If the point is inside the cone, the point visual will be Cyan, if it is outside it will be red. The lines from the point to the cone are Yellow. When attached, the component will add 32 random points to `Points` that are 4 units away.

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This game element is a debug item. Elements like this may be removed at any time without warning, and creations should not rely on it.


## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Height` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The height of the cone. |
| `Radius` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The radius of the cone base. |
| `Points` | _direct_ **[SyncFieldList\`1](https://wiki.resonite.com/Type:SyncFieldList%601 "Type:SyncFieldList`1") < [Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3") >** | Points that the Debug visual will draw lines to from the cone surface to the point. |

Fields
Collapse

## Usage

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:DebugConeDistance&oldid=96406](https://wiki.resonite.com/index.php?title=Component:DebugConeDistance&oldid=96406)"

Contents