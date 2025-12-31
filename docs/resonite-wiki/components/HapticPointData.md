# Component:HapticPointData

> Source: https://wiki.resonite.com/Component:HapticPointData

Collapse **Component image**

[File:HapticPointDataComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=HapticPointDataComponent.png "File:HapticPointDataComponent.png") **Haptic Point Data** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **HapticPointData** component gets data about a haptics device on a particular user.

This works as part of the game's robust [Haptics](https://wiki.resonite.com/Haptics "Haptics") system.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Index` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The device index to get info on. |
| `User` | _direct_ **[UserRef](https://wiki.resonite.com/Type:UserRef "Type:UserRef")** | The user to get a device of `Index` from. |
| `Force` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The device's perceived force. |
| `Temperature` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The device's perceived temperature. |
| `Pain` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The device's perceived pain. |
| `Vibration` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The device's perceived Vibration. |
| `TotalActivationIntensity` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The total activation intensity of the haptic's device. |

Fields
Collapse

## Usage

Attach to a slot and provide a `User` for this component to start giving values.

## Examples

Can be used to create a custom indicator for haptics, or to drive protoflux for haptics.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:HapticPointData&oldid=95924](https://wiki.resonite.com/index.php?title=Component:HapticPointData&oldid=95924)"

Contents