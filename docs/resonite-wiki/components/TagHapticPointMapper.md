# Component:TagHapticPointMapper

> Source: https://wiki.resonite.com/Component:TagHapticPointMapper

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/2/22/TagHapticPointMapperComponent.png/510px-TagHapticPointMapperComponent.png)](https://wiki.resonite.com/File:TagHapticPointMapperComponent.png) **Tag Haptic Point Mapper** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **TagHapticPointMapper** allows for defining custom mapping on avatars.

This works as part of the game's robust [Haptics](https://wiki.resonite.com/Haptics "Haptics") system.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Priority` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The priority of this Mapper over other mappers. |
| `ShowDebugVisuals` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to show the haptic points for this haptic mapper. |
| `HapticPoints` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[TagHapticPointMapper.TaggedHapticPoint](https://wiki.resonite.com/Component:TagHapticPointMapper#TaggedHapticPoint)** | A list of haptic points with tags and where they go. |

Fields
Collapse

## TaggedHapticPoint

| Name | Type | Description |
| --- | --- | --- |
| `HapticTag` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The tag the haptic device needs to be put here. |
| `HapticPointRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | Where to put the haptic sampler for the device. |

Fields

## Usage

By frooxius:

- Full body avatars are automatically instrumented with this component
- You can define list of Slots with associated HapticTag on this component, which determine where will haptic points be mapped to
- You can specify that haptic devices (e.g. GigglePuck) can be mapped to a specific tag in the settings

## Examples

- This gives you flexibility to customize the mapping when it doesn't fit the standard body parametrization, but it requires manual setup on the avatar to configure locations for each [Tag](https://wiki.resonite.com/Tag "Tag").

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:TagHapticPointMapper&oldid=98508](https://wiki.resonite.com/index.php?title=Component:TagHapticPointMapper&oldid=98508)"

Contents