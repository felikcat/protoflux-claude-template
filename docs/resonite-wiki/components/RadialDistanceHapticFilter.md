# Component:RadialDistanceHapticFilter

> Source: https://wiki.resonite.com/Component:RadialDistanceHapticFilter

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/a/a1/RadialDistanceHapticFilterComponent.png/510px-RadialDistanceHapticFilterComponent.png)](https://wiki.resonite.com/File:RadialDistanceHapticFilterComponent.png) **Radial Distance Haptic Filter** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **RadialDistanceHapticFilter** controls haptic areas on the same slot so that haptics within their range are influenced differently depending on how far away they are from the slot center in local space. The start and end intensities when mapped to the haptic devices Distance from the slot, the power is unclamped.

This works as part of the game's robust [Haptics](https://wiki.resonite.com/Haptics "Haptics") system.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `StartRadius` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The starting radius point (Usually 0 distance). When the haptic device point is this Distance away from the slot this component is on in local space, the haptic gets a signal of `Power`\*`StartIntensity` |
| `EndRadius` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The ending radius point (Usually 0 distance). When the haptic device point is this Distance away from the slot this component is on in local space, the haptic gets a signal of `Power`\*`StartIntensity`. |
| `StartIntensity` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The intensity\*`Power` for the haptic device when it is `StartRadius` from the slot this component is on. |
| `EndIntensity` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The intensity\*`Power` for the haptic device when it is `EndRadius` from the slot this component is on. |
| `Power` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to amplify the intensity for the haptic device. |

Fields
Collapse

## Usage

Attach to a slot with a [Component:HapticVolume](https://wiki.resonite.com/Component:HapticVolume "Component:HapticVolume") for the simplest use case. Bringing a user's VR controllers closer or further away changes that device's haptics intensity.

## Examples

Can be used to make an object have an aura that gets more intense as the user goes to grab it.

## See Also

- [Component:HapticVolume](https://wiki.resonite.com/Component:HapticVolume "Component:HapticVolume")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:RadialDistanceHapticFilter&oldid=95908](https://wiki.resonite.com/index.php?title=Component:RadialDistanceHapticFilter&oldid=95908)"

Contents