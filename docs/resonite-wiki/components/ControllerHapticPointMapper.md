# Component:ControllerHapticPointMapper

> Source: https://wiki.resonite.com/Component:ControllerHapticPointMapper

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/a/a6/ControllerHapticPointMapperComponent.png/510px-ControllerHapticPointMapperComponent.png)](https://wiki.resonite.com/File:ControllerHapticPointMapperComponent.png) **Controller Haptic Point Mapper** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ControllerHapticPointMapper** component allows you to specify a point where you feel your controller haptics, this can be useful in cases where you don't feel touching haptic volumes like objects or other user's avatars line up right.

By default without this component, the haptic point is located on the upper end of your controller, which may not desired if your avatar's hands are far away from the end point of your controller.

This works as part of the game's robust [Haptics](https://wiki.resonite.com/Haptics "Haptics") system.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Priority` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The priority of this over other haptic elements |
| `ShowDebugVisuals` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Enables a sphere visual that lights up when touching haptic zones. |
| `Side` | **[Chirality](https://wiki.resonite.com/Type:Chirality "Type:Chirality")** | Specifies which controller/hand this component gives haptic data to. |

Fields
Collapse

## Behavior

The Haptic Point slot from your Controller slot on your Userroot moves underneath the slot where the ControllerHapticPointMapper component is located, which is how this functionality works.

Placing a slot with ControllerHapticPointMapper underneath a user does this behavior instantly, the user does not need to equip their avatar again or respawn.

## Examples

## See Also

- The [Avatar Haptic Source Manager](https://wiki.resonite.com/Component:AvatarHapticSourceManager "Component:AvatarHapticSourceManager") controls the haptic volumes that Haptic Points all use and can be useful if you want to control all aspects of haptics in combination with the Controller Haptic Point Mapper.

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ControllerHapticPointMapper&oldid=97290](https://wiki.resonite.com/index.php?title=Component:ControllerHapticPointMapper&oldid=97290)"

Contents