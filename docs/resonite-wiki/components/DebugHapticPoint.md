# Component:DebugHapticPoint

> Source: https://wiki.resonite.com/Component:DebugHapticPoint

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/8/8c/DebugHapticPointComponent.png/510px-DebugHapticPointComponent.png)](https://wiki.resonite.com/File:DebugHapticPointComponent.png) **Debug Haptic Point** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **DebugHapticPoint** component sends Force sensations to a haptic device as well as gets the name of the haptic device.

This works as part of the game's robust [Haptics](https://wiki.resonite.com/Haptics "Haptics") system.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Intensity` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Sends a sensation of force of this intensity to the Haptic device at `Index` |
| `Index` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The haptic device to send Intensity to and get a name for. |
| `Position` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | The name of the haptic device at `Index` |

Fields
Collapse

## Usage

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:DebugHapticPoint&oldid=95930](https://wiki.resonite.com/index.php?title=Component:DebugHapticPoint&oldid=95930)"

Contents