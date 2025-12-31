# Component:LocomotionGrip

> Source: https://wiki.resonite.com/Component:LocomotionGrip

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/f/f9/LocomotionGripComponent.png/510px-LocomotionGripComponent.png)](https://wiki.resonite.com/File:LocomotionGripComponent.png) **Locomotion Grip** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The LocomotionGrip component controls if users can climb on a collider hierarchy.

For some locomotions, colliders have to specifically be tagged as being climbable. In these cases, this component is used for that purpose.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |

Fields
Collapse

## Usage

While this component is enabled on a slot the hierarchy will be climbable, while this component is disabled on a slot the hierarchy will not be climbable even if climbing is enabled by default in the locomotion.

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:LocomotionGrip&oldid=94890](https://wiki.resonite.com/index.php?title=Component:LocomotionGrip&oldid=94890)"

Contents