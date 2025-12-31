# Component:RandomEventGenerator

> Source: https://wiki.resonite.com/Component:RandomEventGenerator

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/f/f8/RandomEventGeneratorComponent.png/510px-RandomEventGeneratorComponent.png)](https://wiki.resonite.com/File:RandomEventGeneratorComponent.png) **Random Event Generator** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Random event generator is a component that is used to generate random events and point events given a minimum and maximum delay between events.

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `MinInterval` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The minimum time in seconds before another event is generated |
| `MaxInterval` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The maximum time in seconds before another event is generated |
| `RandomPointGenerator` | **[IPointGenerator](https://wiki.resonite.com/Type:IPointGenerator "Type:IPointGenerator")** | a point generator component that is used as the limiter on where random point events can be located. |
| `Events` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[SyncDelegate\`1](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1") < [Action](https://wiki.resonite.com/Type:Action "Type:Action") >** | Random events that when calling a [Sync Delegate](https://wiki.resonite.com/Sync_Delegate "Sync Delegate") provide no data to it's arguments. |
| `PointEvents` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[SyncDelegate\`1](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1") < [Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") < [Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3") >>** | Random events that when calling a [Sync Delegate](https://wiki.resonite.com/Sync_Delegate "Sync Delegate") provide a [Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3") to it's arguments. |

Fields
Collapse

## Behavior

Generates random events and sends them to the lists of `Events` and `PointEvents`.

## Examples

Can be used with a [RandomAudioClipPlayer](https://wiki.resonite.com/Component:RandomAudioClipPlayer "Component:RandomAudioClipPlayer")`PlayAtPoint(Float3 point)` sync delegate to play noises randomly at random points from `RandomPointGenerator` without using [ProtoFlux](https://wiki.resonite.com/ProtoFlux "ProtoFlux").

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:RandomEventGenerator&oldid=91426](https://wiki.resonite.com/index.php?title=Component:RandomEventGenerator&oldid=91426)"

Contents