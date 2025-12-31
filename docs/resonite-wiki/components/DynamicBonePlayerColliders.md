# Component:DynamicBonePlayerColliders

> Source: https://wiki.resonite.com/Component:DynamicBonePlayerColliders

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/9/94/DynamicBonePlayerCollidersComponent.png/510px-DynamicBonePlayerCollidersComponent.png)](https://wiki.resonite.com/File:DynamicBonePlayerCollidersComponent.png) **Dynamic Bone Player Colliders** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

This component is used in the Resonite hair dryer, and allows for dynamic bone colliders specified in the `Colliders` list to automatically collide with [Dynamic Bone Chains](https://wiki.resonite.com/Component:DynamicBoneChain "Component:DynamicBoneChain").

Can also be used in disabling the automatic dynamic bone colliders that Resonite generates incase you want to manually specify them.

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `VisualizeColliders` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Visualize all the colliders in `Colliders` that are currently colliding against a Dynamic Bone Chain. Automatically updates the collider visuals every frame server side. |
| `DisableDefaultHeadColliders` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to not use the default head collider made by the engine. |
| `DisableDefaultBodyColliders` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to not use the body colliders made by the engine. |
| `DisableDefaultLeftHandColliders` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to not use the left hand collider made by the engine. |
| `DisableDefaultRightHandColliders` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to not use the right hand collider made by the engine. |
| `Colliders` | _[list](https://wiki.resonite.com/Type:SyncRefList%601 "Type:SyncRefList`1")_ of **[IDynamicBoneCollider](https://wiki.resonite.com/Type:IDynamicBoneCollider "Type:IDynamicBoneCollider")** | A list of colliders to enable collision for all Dynamic bone chains in a world. |

Fields
Collapse

## Behavior

Only works while the component has an active user.

## Examples

This component is used in the Resonite hair dryer.

## See Also

- [Component:DynamicBoneChain](https://wiki.resonite.com/Component:DynamicBoneChain "Component:DynamicBoneChain")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:DynamicBonePlayerColliders&oldid=100729](https://wiki.resonite.com/index.php?title=Component:DynamicBonePlayerColliders&oldid=100729)"

Contents