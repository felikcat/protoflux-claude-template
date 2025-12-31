# Component:LocomotionAnimationHandMetrics

> Source: https://wiki.resonite.com/Component:LocomotionAnimationHandMetrics

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/3/37/LocomotionAnimationHandMetricsComponent.png/510px-LocomotionAnimationHandMetricsComponent.png)](https://wiki.resonite.com/File:LocomotionAnimationHandMetricsComponent.png) **Locomotion Animation Hand Metrics** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **LocomotionAnimationHandMetrics** component can be used to adjust the settings on the hands for an avatar for its rest state.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Space` | **[LocomotionMetricsSpace](https://wiki.resonite.com/index.php?title=Type:LocomotionMetricsSpace&action=edit&redlink=1 "Type:LocomotionMetricsSpace (page does not exist)")** | What transform space the metric values are in for this component. |
| `ShoulderSeparation` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | An optional value to specify how apart the shoulders are in local space meters. |
| `ShoulderHeight` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | An optional value to specify how far the shoulders are from the ground in local space meters. |
| `ShoulderOffset` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | The offset of the shoulders forwards or backwards in meters. |
| `HandOffset` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | An optional value to specify how far the hands should be offseted from the avatar center in local space meters. |
| `ArmLength` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | An optional value to specify how long the arms are in local space meters. |
| `HandPalmDistance` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | An optional value to specify how long the palms are in local space meters. |

Fields
Collapse

## Usage

Can be used to adjust the arms rest state so they don't collide with the legs or hips too much.

## Examples

Found on the root of avatars set up with the [Avatar Creator](https://wiki.resonite.com/Avatar_Creator "Avatar Creator").

## See Also

- [Component:Locomotion Animation Feet Metrics](https://wiki.resonite.com/Component:LocomotionAnimationFeetMetrics "Component:LocomotionAnimationFeetMetrics")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:LocomotionAnimationHandMetrics&oldid=105305](https://wiki.resonite.com/index.php?title=Component:LocomotionAnimationHandMetrics&oldid=105305)"

Contents