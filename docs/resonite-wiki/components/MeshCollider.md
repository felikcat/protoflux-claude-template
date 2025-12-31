# Component:MeshCollider

> Source: https://wiki.resonite.com/Component:MeshCollider

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:MeshCollider&diff=99072) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/b/b4/MeshColliderComponent.png/510px-MeshColliderComponent.png)](https://wiki.resonite.com/File:MeshColliderComponent.png) **Mesh Collider** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

A mesh collider allows for making a 1:1 collider of the given `Mesh`.

![](https://wiki.resonite.com/images/b/b7/DangerIcon.svg)

Too many polygons colliding with a single collider at once can cause immense frame rate drops. Make sure the geometry on a given mesh collider is not concentrated in a small spot or too dense to avoid this!


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
| `Mesh` | **[Mesh](https://wiki.resonite.com/Type:Mesh "Type:Mesh")** | The mesh to make a collision shape made of groups of polygons out of. |
| `Sidedness` | **[MeshColliderSidedness](https://wiki.resonite.com/Type:MeshColliderSidedness "Type:MeshColliderSidedness")** | Front or back sided collisions. |
| `ActualSpeculativeMargin` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Essentially the room for error on the collisions for this collider. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `ConvexDecomposition:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the create convex hull decomposition button is touched. |
| `ReplaceWithBox:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the replace with box collider button is touched. |

Triggers
Collapse

## Usage

General practice is to use mesh colliders very sparingly.

## Examples

This can be used for more complex collisions like sprawling terrain or procedural meshes that have complex shapes.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:MeshCollider&oldid=99072](https://wiki.resonite.com/index.php?title=Component:MeshCollider&oldid=99072)"

Contents