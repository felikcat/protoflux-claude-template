# Component:DirectTagHapticSource

> Source: https://wiki.resonite.com/Component:DirectTagHapticSource

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/1/19/DirectTagHapticSourceComponent.png/510px-DirectTagHapticSourceComponent.png)](https://wiki.resonite.com/File:DirectTagHapticSourceComponent.png) **Direct Tag Haptic Source** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **DirectTagHapticsSource** component allows driving haptic sensations for a given haptic point directly, rather than using the haptic volume system.

This works as part of the game's robust [Haptics](https://wiki.resonite.com/Haptics "Haptics") system.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `HapticTag` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The tag to influence. |
| `Force` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The force addition for haptics with the `HapticTag` tag. |
| `Temperature` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The temperature addition for haptics with the `HapticTag` tag. |
| `Pain` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The pain addition for haptics with the `HapticTag` tag. |
| `Vibration` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The vibration addition for haptics with the `HapticTag` tag. |

Fields
Collapse

## Usage

- works only with tagged haptic points. This component must have a matching [Tag](https://wiki.resonite.com/Tag "Tag") to a configured haptic device and must be present under the user to work
- It doesn't prevent the haptic volumes from sending haptics - the effects are additive. If you want only this component to control the haptics, do not setup a corresponding tagged haptic point

## Examples

- This can be useful to drive haptics using arbitrary mechanisms (e.g. driving with ProtoFlux), such as grabbing ear/tail dynamic bones, syncing them to world audio reactivity and so on

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:DirectTagHapticSource&oldid=98509](https://wiki.resonite.com/index.php?title=Component:DirectTagHapticSource&oldid=98509)"

Contents