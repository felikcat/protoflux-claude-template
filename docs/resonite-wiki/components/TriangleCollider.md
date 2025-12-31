# Component:TriangleCollider

> Source: https://wiki.resonite.com/Component:TriangleCollider

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/f/f2/TriangleColliderComponent.png/510px-TriangleColliderComponent.png)](https://wiki.resonite.com/File:TriangleColliderComponent.png) **Triangle Collider** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

Triangle collider is a component that acts as a single polygon version of a [Mesh Collider](https://wiki.resonite.com/Component:MeshCollider "Component:MeshCollider")

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Offset` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | how much to add to points `A`, `B`, and `C`. |
| `Type` | **[ColliderType](https://wiki.resonite.com/Type:ColliderType "Type:ColliderType")** | The type of collider. See the enum page for details. |
| `Mass` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How heavy this collider is in total. [according to ProbablePrime](https://discord.com/channels/1040316820650991766/1154514007479287942/1212229273738412082) this is in 1 KG per cubic meter. |
| `CharacterCollider` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether an avatar should be prevented from moving into the collider's volume. |
| `IgnoreRaycasts` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether an avatar's laser should be prevented from hitting the collider's volume. Also this applies to raycasting nodes or components. |
| `A` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The position of the first vertex of the triangle. |
| `B` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The position of the second vertex of the triangle. |
| `C` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The position of the third vertex of the triangle. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `ReverseWinding:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Reverses the order of the vertex values so the face direction is flipped. |

Triggers
Collapse

## Usage

## Examples

This can be used for making a mesh editor.

## See Also

- [Colliders](https://wiki.resonite.com/Collider "Collider")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:TriangleCollider&oldid=100744](https://wiki.resonite.com/index.php?title=Component:TriangleCollider&oldid=100744)"

Contents