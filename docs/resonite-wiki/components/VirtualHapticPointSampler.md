# Component:VirtualHapticPointSampler

> Source: https://wiki.resonite.com/Component:VirtualHapticPointSampler

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/3/3b/VirtualHapticPointSamplerComponent.png/510px-VirtualHapticPointSamplerComponent.png)](https://wiki.resonite.com/File:VirtualHapticPointSamplerComponent.png) **Virtual Haptic Point Sampler** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

Virtual Haptic Point sampler is a component that is used as a way of picking up haptic sensations from the virtual environment inside [Resonite](https://wiki.resonite.com/Resonite "Resonite"), without needing a haptic device. This can be used as a way of making a device that beeps as it detects vibrations, temperature, pain, and force. It can also be used as a way of relaying vibration sensations via API to vibration devices not supported by Resonite, like speakers with base.

This works as part of the game's robust [Haptics](https://wiki.resonite.com/Haptics "Haptics") system.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Radius` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The radius of the sphere for this. |
| `ShowDebugVisual` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to show the debug visual for this sampler. |
| `_debugVisual` | _direct_ **[SlotCleanupRef\`1](https://wiki.resonite.com/index.php?title=Type:SlotCleanupRef%601&action=edit&redlink=1 "Type:SlotCleanupRef`1 (page does not exist)") < [OverlayFresnelMaterial](https://wiki.resonite.com/OverlayFresnelMaterial "OverlayFresnelMaterial") >** | the material on the sphere of the current generated debug visual. Is null when `ShowDebugVisual` is false. |
| `Force` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The force sensations picked up by this haptic point sampler. |
| `Pain` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The pain sensations picked up by this haptic point sampler. |
| `Temperature` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The temperature sensations picked up by this haptic point sampler. |
| `Vibration` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | the vibration sensations picked up by this haptic point sampler. |

Fields
Collapse

## Usage

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This component will do nothing locally unless the user has haptic feedback enabled in their settings!


## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:VirtualHapticPointSampler&oldid=95920](https://wiki.resonite.com/index.php?title=Component:VirtualHapticPointSampler&oldid=95920)"

Contents