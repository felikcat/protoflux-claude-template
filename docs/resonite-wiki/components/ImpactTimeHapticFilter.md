# Component:ImpactTimeHapticFilter

> Source: https://wiki.resonite.com/Component:ImpactTimeHapticFilter

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/0/0c/ImpactTimeHapticFilterComponent.png/510px-ImpactTimeHapticFilterComponent.png)](https://wiki.resonite.com/File:ImpactTimeHapticFilterComponent.png) **Impact Time Haptic Filter** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ImpactTimeHapticFilter** component is a haptics filter mainly for [Component:HapticVolumes](https://wiki.resonite.com/Component:HapticVolume "Component:HapticVolume") change their intensity based on how long the user's hand has been inside of the affecting area.

This works as part of the game's robust [Haptics](https://wiki.resonite.com/Haptics "Haptics") system.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `UseGlobalTime` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to use global time or local time. |
| `StartTime` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | When the user's hand has been here for this amount of time, use `StartIntensity`. |
| `EndTime` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | When the user's hand has been here for this amount of time, use `EndIntensity`. |
| `StartIntensity` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The intensity to use at the start of the time frame. |
| `EndIntensity` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The intensity to use at the end of the time frame. |
| `Power` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to amplify the overall intensity effect of this component. |

Fields
Collapse

## Usage

Attach to a slot with a valid and working [Component:HapticVolume](https://wiki.resonite.com/Component:HapticVolume "Component:HapticVolume") to add to the list of multiplicative haptic filters.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ImpactTimeHapticFilter&oldid=96131](https://wiki.resonite.com/index.php?title=Component:ImpactTimeHapticFilter&oldid=96131)"

Contents