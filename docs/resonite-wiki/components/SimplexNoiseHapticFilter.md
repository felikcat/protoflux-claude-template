# Component:SimplexNoiseHapticFilter

> Source: https://wiki.resonite.com/Component:SimplexNoiseHapticFilter

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/4/4e/SimplexNoiseHapticFilterComponent.png/510px-SimplexNoiseHapticFilterComponent.png)](https://wiki.resonite.com/File:SimplexNoiseHapticFilterComponent.png) **Simplex Noise Haptic Filter** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **SimplexNoiseHapticFilter** makes the space within a collider with [haptic volume](https://wiki.resonite.com/Component:HapticVolume "Component:HapticVolume") act like a 3d noise kind of like moving your haptics device through clouds.

This works as part of the game's robust [Haptics](https://wiki.resonite.com/Haptics "Haptics") system.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `NoiseScale` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The scale of the noise. |
| `NoiseOffset` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The offset of the noise from 0. |
| `MinValue` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The minimum haptics power the noise can give based on the 3d noise algorithm. |
| `MaxValue` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The maximum haptics power the noise can give based on the 3d noise algorithm. |

Fields
Collapse

## Usage

Attach to a slot with a [HapticVolume](https://wiki.resonite.com/Component:HapticVolume "Component:HapticVolume") and a collider. This component will then start working.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Component:HapticVolume](https://wiki.resonite.com/Component:HapticVolume "Component:HapticVolume")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:SimplexNoiseHapticFilter&oldid=95910](https://wiki.resonite.com/index.php?title=Component:SimplexNoiseHapticFilter&oldid=95910)"

Contents