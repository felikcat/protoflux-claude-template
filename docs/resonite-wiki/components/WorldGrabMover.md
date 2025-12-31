# Component:WorldGrabMover

> Source: https://wiki.resonite.com/Component:WorldGrabMover

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/f/fa/WorldGrabMoverComponent.png/510px-WorldGrabMoverComponent.png)](https://wiki.resonite.com/File:WorldGrabMoverComponent.png) **World Grab Mover** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **WorldGrabMover** component is used as a visual for the [grab world locomotion](https://wiki.resonite.com/Component:GrabWorldLocomotion "Component:GrabWorldLocomotion").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `ShowLerp` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The lerp value for showing the visual. |
| `_activatingUser` | **[User](https://wiki.resonite.com/Type:User "Type:User")** | The user making this visual for grabbing onto the world. |
| `_crossMesh` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[CrossMesh](https://wiki.resonite.com/Component:CrossMesh "Component:CrossMesh")** | The cross mesh being used for the anchor visual. |
| `_visualVisible` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the visual should be visible. |
| `_visualRotation` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The field to drive with the rotation for the visual. |
| `_material` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[PBS\_RimMetallic](https://wiki.resonite.com/PBS_RimMetallic "PBS RimMetallic")** | The material that the visual is using. |
| `_referencePosition` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | the position this visual is trying to stay and anchor at. |

Fields
Collapse

## Usage

Not used directly by the user.

## Examples

The cross that appears on the user's hand when moving with [grab world locomotion](https://wiki.resonite.com/Component:GrabWorldLocomotion "Component:GrabWorldLocomotion").

## See Also

- [Component:GrabWorldLocomotion](https://wiki.resonite.com/Component:GrabWorldLocomotion "Component:GrabWorldLocomotion")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:WorldGrabMover&oldid=100827](https://wiki.resonite.com/index.php?title=Component:WorldGrabMover&oldid=100827)"

Contents