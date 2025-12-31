# Component:ValueNoiseHapticFilter

> Source: https://wiki.resonite.com/Component:ValueNoiseHapticFilter

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/b/b9/ValueNoiseHapticFilterComponent.png/510px-ValueNoiseHapticFilterComponent.png)](https://wiki.resonite.com/File:ValueNoiseHapticFilterComponent.png) **Value Noise Haptic Filter** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ValueNoiseHapticFilter** component makes a random intensity value every update to a device touching a [Component:HapticVolume](https://wiki.resonite.com/Component:HapticVolume "Component:HapticVolume").

This works as part of the game's robust [Haptics](https://wiki.resonite.com/Haptics "Haptics") system.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `MinValue` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The minimum haptic intensity to output in a game tick. |
| `MaxValue` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The maximum haptic intensity to output in a game tick. |

Fields
Collapse

## Usage

Attach to a slot with a valid and working [Component:HapticVolume](https://wiki.resonite.com/Component:HapticVolume "Component:HapticVolume") to add to the list of multiplicative haptic filters.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Component:HapticVolume](https://wiki.resonite.com/Component:HapticVolume "Component:HapticVolume")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ValueNoiseHapticFilter&oldid=95911](https://wiki.resonite.com/index.php?title=Component:ValueNoiseHapticFilter&oldid=95911)"

Contents