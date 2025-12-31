# Component:BoxCollider

> Source: https://wiki.resonite.com/Component:BoxCollider

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:BoxCollider&diff=97880) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/0/0a/BoxColliderComponent.png/510px-BoxColliderComponent.png)](https://wiki.resonite.com/File:BoxColliderComponent.png) **Box Collider** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

Representing a simple box, this collider is the second most performant collider in the game, beaten by [Sphere Colliders](https://wiki.resonite.com/Component:SphereCollider "Component:SphereCollider")

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
| `Size` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | How big locally this collider is in the x, y, and z directions. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `SetFromLocalBounds:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Gathers all objects and slots under this component's slot, creates a Bounding box that encapsulates all the points and Bounding boxes, and uses the Bounding box to set this component's values. Does all calculations in local space. |
| `SetFromGlobalBounds:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Gathers all objects and slots under this component's slot, creates a Bounding box that encapsulates all the points and Bounding boxes, and uses the Bounding box to set this component's values. Does all calculations in global space. |
| `SetFromLocalBounds:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Gathers all objects and slots under this component's slot, creates a Bounding box that encapsulates all the points and Bounding boxes, and uses the Bounding box to set this component's values. Does all calculations in local space. |
| `SetFromGlobalBounds:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Gathers all objects and slots under this component's slot, creates a Bounding box that encapsulates all the points and Bounding boxes, and uses the Bounding box to set this component's values. Does all calculations in global space. |
| `SetFromLocalBoundsPrecise:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Gathers all objects and slots under this component's slot, creates a Bounding box that encapsulates all the points and Bounding boxes, and uses the Bounding box to set this component's values. Does all calculations in local space. Ignores floating point error. |
| `SetFromGlobalBoundsPrecise:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Gathers all objects and slots under this component's slot, creates a Bounding box that encapsulates all the points and Bounding boxes, and uses the Bounding box to set this component's values. Does all calculations in global space. Ignores floating point error. |

Triggers
Collapse

## Usage

This is useful for floors and walls, and can also be set to NoCollide and used as a way to mark an area for a custom culling system.

## Examples

## See Also

- [Collider](https://wiki.resonite.com/Collider "Collider")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:BoxCollider&oldid=97880](https://wiki.resonite.com/index.php?title=Component:BoxCollider&oldid=97880)"

Contents