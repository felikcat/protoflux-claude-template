# Component:SineHapticFilter

> Source: https://wiki.resonite.com/Component:SineHapticFilter

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/9/92/SineHapticFilterComponent.png/510px-SineHapticFilterComponent.png)](https://wiki.resonite.com/File:SineHapticFilterComponent.png) **Sine Haptic Filter** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **SineHapticFilter** component is used to make haptics triggered by Components on the same slot change in intensity over time like its riding waves.

This works as part of the game's robust [Haptics](https://wiki.resonite.com/Haptics "Haptics") system.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `UseGlobalTime` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to use the global time or the initial local time for initial time when touched. |
| `DistanceScale` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | An optional value on how to add to the offset in time for the waves of intensity based on distance of the haptic device from the slot this component is on. |
| `AxisScale` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3") >** | An optional value on how to add to the offset in time for the waves of intensity based on how close it is to a line direction in local space. |
| `MinIntensity` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The minimum haptics intensity this component will send. |
| `MaxIntensity` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The maximum haptics intensity this component will send. |
| `Frequency` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The speed at which the sinewave goes up and down over time. |

Fields
Collapse

## Usage

Attach to a slot with a [HapticVolume](https://wiki.resonite.com/Component:HapticVolume "Component:HapticVolume") and a collider. This component will then start working.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Component:HapticVolume](https://wiki.resonite.com/Component:HapticVolume "Component:HapticVolume")
- [Haptics](https://wiki.resonite.com/Haptics "Haptics")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:SineHapticFilter&oldid=95906](https://wiki.resonite.com/index.php?title=Component:SineHapticFilter&oldid=95906)"

Contents