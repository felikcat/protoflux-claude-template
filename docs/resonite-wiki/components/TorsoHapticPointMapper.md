# Component:TorsoHapticPointMapper

> Source: https://wiki.resonite.com/Component:TorsoHapticPointMapper

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/b/b9/TorsoHapticPointMapperComponent.png/510px-TorsoHapticPointMapperComponent.png)](https://wiki.resonite.com/File:TorsoHapticPointMapperComponent.png) **Torso Haptic Point Mapper** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **TorsoHapticPointMapper** component is used to tell the game the size of an Avatar's torso and its bones in order for the game to know where to place haptic point samplers so they better match the size and positions of the body.

The area makes up a 3d trapezoid with thickness, with a parallel front and back, and top and bottom, but a non parallel left and right.

This works as part of the game's robust [Haptics](https://wiki.resonite.com/Haptics "Haptics") system.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Priority` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The priority of this Mapper over other mappers. |
| `ShowDebugVisuals` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to show the area and haptic point Debug visuals. |
| `BoneChain` | _[list](https://wiki.resonite.com/Type:SyncRefList%601 "Type:SyncRefList`1")_ of **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | A list of bones that make up the center spine of the avatar. (Hips, Spine(s), Chest, upper chest) |
| `NormalizedStart` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Where in the chain does the haptics mapping start? |
| `NormalizedEnd` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Where in the chain does the haptics mapping end? |
| `LowerWidth` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The width of the lower spine. |
| `UpperWidth` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The width of the upper spine. |
| `FrontOffset` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How far the front side is from the spine bones. |
| `BackOffset` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How far the back side is from the spine bones. |

Fields
Collapse

## Usage

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Examples

Attached to the chest of an avatar set up with the [Avatar Creator](https://wiki.resonite.com/Avatar_Creator "Avatar Creator") in order for the avatar to handle mapping haptics to its surface correctly for things like haptics vests or giggle pucks.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:TorsoHapticPointMapper&oldid=95918](https://wiki.resonite.com/index.php?title=Component:TorsoHapticPointMapper&oldid=95918)"

Contents