# Component:AxisDistanceHapticFilter

> Source: https://wiki.resonite.com/Component:AxisDistanceHapticFilter

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/d/d4/AxisDistanceHapticFilterComponent.png/510px-AxisDistanceHapticFilterComponent.png)](https://wiki.resonite.com/File:AxisDistanceHapticFilterComponent.png) **Axis Distance Haptic Filter** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **AxisDistanceHapticFilter** multiplicatively changes the intensity of a [Component:HapticVolume](https://wiki.resonite.com/Component:HapticVolume "Component:HapticVolume") depending on the dot product from the vector of the device's position in local space to this component and `Axis`. Essentially the smaller the angle between the device local position from 0 direction and the `Axis` direction the smaller the distance.

This works as part of the game's robust [Haptics](https://wiki.resonite.com/Haptics "Haptics") system.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Axis` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The axis to check distance from. |
| `StartDistance` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The starting distance to map to `StartIntensity` for the intensity distance range. |
| `EndDistance` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The ending distance to map to `EndIntensity` for the intensity distance range. |
| `StartIntensity` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | When at `StartDistance` map the device intensity to this. |
| `EndIntensity` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | When at `EndDistance` map the device intensity to this. |
| `Power` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to amplify the haptics effect in general. |

Fields
Collapse

## Usage

Attach to a slot with a valid and working [Component:HapticVolume](https://wiki.resonite.com/Component:HapticVolume "Component:HapticVolume") to add to the list of multiplicative haptic filters.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AxisDistanceHapticFilter&oldid=95932](https://wiki.resonite.com/index.php?title=Component:AxisDistanceHapticFilter&oldid=95932)"

Contents