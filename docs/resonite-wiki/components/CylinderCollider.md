# Component:CylinderCollider

> Source: https://wiki.resonite.com/Component:CylinderCollider

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/7/78/CylinderColliderComponent.png/510px-CylinderColliderComponent.png)](https://wiki.resonite.com/File:CylinderColliderComponent.png) **Cylinder Collider** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

Is like a [Capsule Collider](https://wiki.resonite.com/Component:CapsuleCollider "Component:CapsuleCollider") except instead of rounded ends the ends are flat.

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
| `Height` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Height of the cylinder shape of the collider |
| `Radius` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The radius of the cylinder shape of the collider from center to edge. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `SetFromPreciseBounds:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Gathers all objects and slots under this component's slot, creates a Bounding box that encapsulates all the points and Bounding boxes, and uses the Bounding box to set this component's values. Does all calculations in local space. Ignores floating point error. |
| `SetFromPreciseBounds:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Gathers all objects and slots under this component's slot, creates a Bounding box that encapsulates all the points and Bounding boxes, and uses the Bounding box to set this component's values. Does all calculations in local space. Ignores floating point error. |

Triggers
Collapse

## Usage

Can be used for a greek pillar in a room.

## Examples

## See Also

[Issue 1087](https://github.com/Yellow-Dog-Man/Resonite-Issues/issues/1087)

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:CylinderCollider&oldid=97912](https://wiki.resonite.com/index.php?title=Component:CylinderCollider&oldid=97912)"

Contents