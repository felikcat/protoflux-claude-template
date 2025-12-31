# Component:HapticVolume

> Source: https://wiki.resonite.com/Component:HapticVolume

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/1/19/HapticVolumeComponent.png/510px-HapticVolumeComponent.png)](https://wiki.resonite.com/File:HapticVolumeComponent.png) **Haptic Volume** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

Haptic Volumes allows a user to feel haptics through a [collider](https://wiki.resonite.com/Collider "Collider") set to Haptic Trigger shared on the same slot.

Haptic Volumes can be paired with [Haptic Filters](https://wiki.resonite.com/Category:Components:Input:Haptics:Filters "Category:Components:Input:Haptics:Filters") placed on the same slot to give more precise control over a user's haptics. Each haptic filter is applied by multiplying each influence together, hence being multiplicative.

This works as part of the game's robust [Haptics](https://wiki.resonite.com/Haptics "Haptics") system.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Sensation` | **[SensationClass](https://wiki.resonite.com/Type:SensationClass "Type:SensationClass")** | The type of haptic you want to do, for controllers the haptic types are subtly different variations. Specifying this is useful for haptic suits that have more advanced haptic motors. |
| `Intensity` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The haptic intensity ranging from zero to one, zero being none one being max that the device allows. |
| `SensationHints` | _direct_ **[SyncFieldList\`1](https://wiki.resonite.com/Type:SyncFieldList%601 "Type:SyncFieldList`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | Allows triggering specific predefined sensations with certain haptic devices. Only useful for OWO haptic vests currently. |

Fields
Collapse

## Usage

When placed on a slot with a [collider](https://wiki.resonite.com/Collider "Collider") component, the collider's type automatically switches to haptic trigger.

## Examples

## See Also

- [Avatar Haptic Source Manager](https://wiki.resonite.com/Component:AvatarHapticSourceManager "Component:AvatarHapticSourceManager") that directly controls haptic volumes for custom avatar defined haptics.

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:HapticVolume&oldid=95931](https://wiki.resonite.com/index.php?title=Component:HapticVolume&oldid=95931)"

Contents