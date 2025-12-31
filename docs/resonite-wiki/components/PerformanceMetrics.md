# Component:PerformanceMetrics

> Source: https://wiki.resonite.com/Component:PerformanceMetrics

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/0/00/PerformanceMetricsComponent.png/510px-PerformanceMetricsComponent.png)](https://wiki.resonite.com/File:PerformanceMetricsComponent.png) **Performance Metrics** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **PerformanceMetrics** component is used to show performance for a particular `User` at the present moment.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `User` | _direct_ **[UserRef](https://wiki.resonite.com/Type:UserRef "Type:UserRef")** | The user we are measuring performance for. |
| `FPS` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | `User`'s Frames Per second. |
| `ImmediateFPS` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | `User`'s immediate Frames Per Second. |
| `RenderTime` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | `User`'s time it takes to render the scene in seconds. |
| `TotalEngineUpdateTime` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | `User`'s time it takes to update the engine in seconds. |

Fields
Collapse

## Usage

Attach to a slot and provide a user for `User` for it to start giving performance metrics.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:PerformanceMetrics&oldid=95411](https://wiki.resonite.com/index.php?title=Component:PerformanceMetrics&oldid=95411)"

Contents