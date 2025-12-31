# Component:ConvexHullCollider

> Source: https://wiki.resonite.com/Component:ConvexHullCollider

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/d/df/ConvexHullColliderComponent.png/510px-ConvexHullColliderComponent.png)](https://wiki.resonite.com/File:ConvexHullColliderComponent.png) **Convex Hull Collider** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

Is a [convex hull](https://en.wikipedia.org/wiki/Convex_hull) (a shape closely wrapping the object, but with no indentations) over the mesh of the object.

## Usage

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
| `Mesh` | **[Mesh](https://wiki.resonite.com/Type:Mesh "Type:Mesh")** | The mesh to wrap (kind of like using plastic wrap) and use the wrapped result as the collider this component represents. |

Fields
Collapse

## Behavior

## Examples

Can be used to simplify mesh colliders like an elongated sphere, where keeping the object concave isn't important.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ConvexHullCollider&oldid=91057](https://wiki.resonite.com/index.php?title=Component:ConvexHullCollider&oldid=91057)"

Contents