# Component:LocomotionAnimationFeetMetrics

> Source: https://wiki.resonite.com/Component:LocomotionAnimationFeetMetrics

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/1/14/LocomotionAnimationFeetMetricsComponent.png/510px-LocomotionAnimationFeetMetricsComponent.png)](https://wiki.resonite.com/File:LocomotionAnimationFeetMetricsComponent.png) **Locomotion Animation Feet Metrics** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **LocomotionAnimationFeetMetrics** component is used to adjust the settings for an avatar's feet.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Space` | **[LocomotionMetricsSpace](https://wiki.resonite.com/index.php?title=Type:LocomotionMetricsSpace&action=edit&redlink=1 "Type:LocomotionMetricsSpace (page does not exist)")** | What transform space the metric values are in for this component. |
| `FeetSeparation` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | How far apart the feet should be placed from each other. |
| `FeetBackwardsOffset` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | How much the foot should be shifted forwards or backwards. |
| `FootHeight` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | The distance from the floor to the foot bone for the whole foot. |
| `FootFrontOffset` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | An optional value to influence the foot front distance from floor value. |
| `FootBackOffset` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | An optional value to influence the foot back distance from floor value. |

Fields
Collapse

## Usage

## Examples

Appears on the root of avatars created by the [Avatar Creator](https://wiki.resonite.com/Avatar_Creator "Avatar Creator").

## See Also

- [Component:Locomotion Animation Hand Metrics](https://wiki.resonite.com/Component:LocomotionAnimationHandMetrics "Component:LocomotionAnimationHandMetrics")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:LocomotionAnimationFeetMetrics&oldid=104700](https://wiki.resonite.com/index.php?title=Component:LocomotionAnimationFeetMetrics&oldid=104700)"

Contents