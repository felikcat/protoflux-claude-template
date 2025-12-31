# Component:CylindricalDistanceHapticFilter

> Source: https://wiki.resonite.com/Component:CylindricalDistanceHapticFilter

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/e/e1/CylindricalDistanceHapticFilterComponent.png/510px-CylindricalDistanceHapticFilterComponent.png)](https://wiki.resonite.com/File:CylindricalDistanceHapticFilterComponent.png) **Cylindrical Distance Haptic Filter** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **CylindricalDistanceHapticFilter** component filters haptic device influences multiplicatively depending on their position within a range of 2 cylinders. One being an inner and one being an outer. Both of them are invisible though. This component works when used with a [Component:HapticVolume](https://wiki.resonite.com/Component:HapticVolume "Component:HapticVolume").

This works as part of the game's robust [Haptics](https://wiki.resonite.com/Haptics "Haptics") system.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `StartRadius` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The starting radius of the intensity gradient based on distance from the cylinders center line from end to end. |
| `EndRadius` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The ending radius of the intensity gradient based on distance from the cylinders center line from end to end. |
| `StartRadiusIntensity` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The starting intensity of the intensity gradient based on distance from the cylinders center line from end to end. |
| `EndRadiusIntensity` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The ending intensity of the intensity gradient based on distance from the cylinders center line from end to end. |
| `RadiusPower` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The amplification of the intensity gradient based on distance from the cylinders center line from end to end. |
| `StartAxisOffset` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Used to define the distance from the cylinder end cap to start the intensity gradient. |
| `EndAxisOffset` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Used to define the distance from the cylinder end cap to end the intensity gradient. |
| `StartAxisIntensity` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The starting intensity value for the intensity gradient based on the distance to the cylinder cap. |
| `EndAxisIntensity` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The ending intensity value for the intensity gradient based on the distance to the cylinder cap. |
| `AxisPower` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to amplify the intensity of the intensity gradient based on the distance to the cylinder cap. |

Fields
Collapse

## Usage

Attach to a slot with a valid and working [Component:HapticVolume](https://wiki.resonite.com/Component:HapticVolume "Component:HapticVolume") to add to the list of multiplicative haptic filters.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:CylindricalDistanceHapticFilter&oldid=95934](https://wiki.resonite.com/index.php?title=Component:CylindricalDistanceHapticFilter&oldid=95934)"

Contents