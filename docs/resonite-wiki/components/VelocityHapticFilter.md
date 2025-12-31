# Component:VelocityHapticFilter

> Source: https://wiki.resonite.com/Component:VelocityHapticFilter

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/b/b6/VelocityHapticFilterComponent.png/510px-VelocityHapticFilterComponent.png)](https://wiki.resonite.com/File:VelocityHapticFilterComponent.png) **Velocity Haptic Filter** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **VelocityHapticFilter** component is used to influence the haptics a user feels on a haptics device as the device moves through a [Component:HapticVolume](https://wiki.resonite.com/Component:HapticVolume "Component:HapticVolume") at different speeds.

This works as part of the game's robust [Haptics](https://wiki.resonite.com/Haptics "Haptics") system.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `VelocitySmoothTime` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to smooth the changes in velocity this component works with. |
| `StartVelocity` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The velocity to map to `StartIntensity`. |
| `EndVelocity` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The velocity to map to `EndIntensity`. |
| `StartIntensity` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The intensity to use when a haptics device is moving at `StartVelocity` through a valid [Component:HapticVolume](https://wiki.resonite.com/Component:HapticVolume "Component:HapticVolume") on the same slot. |
| `EndIntensity` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The intensity to use when a haptics device is moving at `EndVelocity` through a valid [Component:HapticVolume](https://wiki.resonite.com/Component:HapticVolume "Component:HapticVolume") on the same slot. |
| `Power` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The multiplier of the haptics intensity before applying it. |

Fields
Collapse

## Usage

Attach to a slot with a valid and working [Component:HapticVolume](https://wiki.resonite.com/Component:HapticVolume "Component:HapticVolume") to add to the list of multiplicative haptic filters.

## Examples

Can be used to make haptics that feel like the user's body is moving through water.

## See Also

- [Component:HapticVolume](https://wiki.resonite.com/Component:HapticVolume "Component:HapticVolume")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:VelocityHapticFilter&oldid=95905](https://wiki.resonite.com/index.php?title=Component:VelocityHapticFilter&oldid=95905)"

Contents