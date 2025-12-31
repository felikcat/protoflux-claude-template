# Component:ArmHapticPointMapper

> Source: https://wiki.resonite.com/Component:ArmHapticPointMapper

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/1/1b/ArmHapticPointMapperComponent.png/510px-ArmHapticPointMapperComponent.png)](https://wiki.resonite.com/File:ArmHapticPointMapperComponent.png) **Arm Haptic Point Mapper** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Arm Haptic Point Mapper** works as part of the game's robust [Haptics](https://wiki.resonite.com/Haptics "Haptics") system to map haptics points in real life for the arm to the in game arms.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Priority` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The priority of this over other haptic elements |
| `ShowDebugVisuals` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Enables a sphere visual that lights up when touching haptic zones. |
| `BoneChain` | _[list](https://wiki.resonite.com/Type:SyncRefList%601 "Type:SyncRefList`1")_ of **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The list of slots to distribute the haptic points along for the arm. |
| `NormalizedStart` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The start of where haptics points should be placed based on a normalized position from 0<->1 along the length of the arm, if all the bones were rotated to be along a straight line. |
| `NormalizedEnd` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The end of where haptics points should be placed based on a normalized position from 0<->1 along the length of the arm, if all the bones were rotated to be along a straight line. |
| `Side` | **[Chirality](https://wiki.resonite.com/Type:Chirality "Type:Chirality")** | Specifies which controller/hand this component gives haptic data to. |
| `UpAxis` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The axis on the arm which determines which way is up per bone, which is used to map haptic points from real life to in game. |
| `ForwardAxis` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The axis on the arm which determines which way is forward per bone, which is used to map haptic points from real life to in game. |
| `HandRadius` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The radius of the hand in which to map haptics points for. |

Fields
Collapse

## Usage

Used in the robust [Haptics](https://wiki.resonite.com/Haptics "Haptics") system to map haptics points in real life for the arm to the in game arms.

## Examples

Found by default on the upper arms of avatars.

## See Also

- [Haptics](https://wiki.resonite.com/Haptics "Haptics")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ArmHapticPointMapper&oldid=103805](https://wiki.resonite.com/index.php?title=Component:ArmHapticPointMapper&oldid=103805)"

Contents