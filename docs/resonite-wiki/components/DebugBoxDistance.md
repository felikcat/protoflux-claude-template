# Component:DebugBoxDistance

> Source: https://wiki.resonite.com/Component:DebugBoxDistance

Collapse **Component image**

[File:DebugBoxDistanceComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=DebugBoxDistanceComponent.png "File:DebugBoxDistanceComponent.png") **Debug Box Distance** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Debug Box Distance** component allows for debugging the distance from a box object, and generates 32 random points on attach to do so.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Size` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The size of the box to debug |
| `Points` | _direct_ **[SyncFieldList\`1](https://wiki.resonite.com/Type:SyncFieldList%601 "Type:SyncFieldList`1") < [Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3") >** | The points to use to visualize the distances from the box. |

Fields
Collapse

## Usage

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:DebugBoxDistance&oldid=101117](https://wiki.resonite.com/index.php?title=Component:DebugBoxDistance&oldid=101117)"

Contents