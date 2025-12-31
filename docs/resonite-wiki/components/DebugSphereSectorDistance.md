# Component:DebugSphereSectorDistance

> Source: https://wiki.resonite.com/Component:DebugSphereSectorDistance

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/d/d3/DebugSphereSectorDistanceComponent.png/510px-DebugSphereSectorDistanceComponent.png)](https://wiki.resonite.com/File:DebugSphereSectorDistanceComponent.png) **Debug Sphere Sector Distance** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **DebugSphereSectorDistance** component makes a bunch of spazzy lines all over the place that vaguely resembles two spheres having a shoot out. This is only used for Debug.

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This game element is a debug item. Elements like this may be removed at any time without warning, and creations should not rely on it.


## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Angle` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The angle of the sphere to debug |
| `Radius` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The radius of the sphere |
| `Points` | _direct_ **[SyncFieldList\`1](https://wiki.resonite.com/Type:SyncFieldList%601 "Type:SyncFieldList`1") < [Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3") >** | A bunch of random points |

Fields
Collapse

## Usage

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:DebugSphereSectorDistance&oldid=96392](https://wiki.resonite.com/index.php?title=Component:DebugSphereSectorDistance&oldid=96392)"

Contents