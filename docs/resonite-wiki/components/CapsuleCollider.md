# Component:CapsuleCollider

> Source: https://wiki.resonite.com/Component:CapsuleCollider

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/b/b8/CapsuleCollider.png/510px-CapsuleCollider.png)](https://wiki.resonite.com/File:CapsuleCollider.png) **Capsule Collider** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The CapsuleCollider component creates a simple capsule collision shape from the defined height and radius.

The CapsuleCollider is used in [Locomotion Modules](https://wiki.resonite.com/Locomotion_Modules_(Slot) "Locomotion Modules (Slot)") to represent the player's width and height.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Offset` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The offset of the collider shape's position from the slot's position. |
| `Type` | **[ColliderType](https://wiki.resonite.com/Type:ColliderType "Type:ColliderType")** | The type of collider. See the enum page for details. |
| `Mass` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How heavy this collider is in total. [according to ProbablePrime](https://discord.com/channels/1040316820650991766/1154514007479287942/1212229273738412082) this is in 1 KG per cubic meter. |
| `CharacterCollider` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether an avatar should be prevented from moving into the collider's volume. |
| `IgnoreRaycasts` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether an avatar's laser should be prevented from hitting the collider's volume. Also this applies to raycasting nodes or components. |
| `Height` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The height of the capsule. Does not include the added height from the rounded ends |
| `Radius` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | the radius of the body of the capsule and it's rounded ends. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `SetFromExactCylinder:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Gathers all objects and slots under this component's slot, creates a Bounding box that encapsulates all the points and Bounding boxes, and uses the Bounding box to set this component's values. Does all calculations in local space. Ignores floating point error. |
| `SetFromExactCylinder:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Gathers all objects and slots under this component's slot, creates a Bounding box that encapsulates all the points and Bounding boxes, and uses the Bounding box to set this component's values. Does all calculations in local space. Ignores floating point error. |

Triggers
Collapse

## Usage

## Examples

## See Also

- [Collider](https://wiki.resonite.com/Collider "Collider")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:CapsuleCollider&oldid=97888](https://wiki.resonite.com/index.php?title=Component:CapsuleCollider&oldid=97888)"

Contents