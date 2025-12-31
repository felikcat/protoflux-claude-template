# Component:HeadHapticPointMapper

> Source: https://wiki.resonite.com/Component:HeadHapticPointMapper

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/5/57/HeadHapticPointMapperComponent.png/510px-HeadHapticPointMapperComponent.png)](https://wiki.resonite.com/File:HeadHapticPointMapperComponent.png) **Head Haptic Point Mapper** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **HeadHapticPointMapper** component handles mapping haptic points around and to the head area of a user.

This works as part of the game's robust [Haptics](https://wiki.resonite.com/Haptics "Haptics") system.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Priority` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The priority of this Mapper over other mappers. |
| `ShowDebugVisuals` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to show the area visual of the Mapper and the different haptics mapped to it. |
| `HeadSize` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | How big the head is. |
| `HeadCenter` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The center offset of the head area compared to the slot this component is on (the head slot) |
| `_debugVisual` | _direct_ **[SlotCleanupRef\`1](https://wiki.resonite.com/index.php?title=Type:SlotCleanupRef%601&action=edit&redlink=1 "Type:SlotCleanupRef`1 (page does not exist)") < [Slot](https://wiki.resonite.com/Type:Slot "Type:Slot") >** | The root slot of the current Debug visual. |

Fields
Collapse

## Usage

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Examples

On the head slot of avatars by default made with the [Avatar Creator](https://wiki.resonite.com/Avatar_Creator "Avatar Creator").

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:HeadHapticPointMapper&oldid=95919](https://wiki.resonite.com/index.php?title=Component:HeadHapticPointMapper&oldid=95919)"

Contents