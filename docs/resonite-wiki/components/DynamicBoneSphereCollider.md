# Component:DynamicBoneSphereCollider

> Source: https://wiki.resonite.com/Component:DynamicBoneSphereCollider

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/9/96/DynamicBoneSphereColliderComponent.png/510px-DynamicBoneSphereColliderComponent.png)](https://wiki.resonite.com/File:DynamicBoneSphereColliderComponent.png) **Dynamic Bone Sphere Collider** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The dynamic bone sphere collider is a component that allows for making a static sphere collider by adding it to the list of `StaticColliders` on a [DynamicBoneChain](https://wiki.resonite.com/Component:DynamicBoneChain "Component:DynamicBoneChain") or make it dynamic by making it part of the `Colliders` list on a [DynamicBonePlayerColliders Component](https://wiki.resonite.com/Component:DynamicBonePlayerColliders "Component:DynamicBonePlayerColliders")

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Radius` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The radius of the sphere created by this component in local space of the [Slot](https://wiki.resonite.com/Slot "Slot") it is made on. |

Fields
Collapse

## Behavior

## Examples

This component can be used with a [RaycastDriver](https://wiki.resonite.com/Component:RaycastDriver "Component:RaycastDriver") to make a huge sphere under the ground that can act as a floor. Then adding this component to the list of static colliders on a [DynamicBoneChain](https://wiki.resonite.com/Component:DynamicBoneChain "Component:DynamicBoneChain") allows for fake collisions with the floor, so tails, wings, chains, and cloth tassles won't clip through the ground on avatars.

## See Also

- [Component:DynamicBoneChain](https://wiki.resonite.com/Component:DynamicBoneChain "Component:DynamicBoneChain")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:DynamicBoneSphereCollider&oldid=93831](https://wiki.resonite.com/index.php?title=Component:DynamicBoneSphereCollider&oldid=93831)"

Contents