# Component:DynamicBoneSphereColliderGizmo

> Source: https://wiki.resonite.com/Component:DynamicBoneSphereColliderGizmo

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/f/fb/DynamicBoneSphereColliderGizmoComponent.png/510px-DynamicBoneSphereColliderGizmoComponent.png)](https://wiki.resonite.com/File:DynamicBoneSphereColliderGizmoComponent.png) **Dynamic Bone Sphere Collider Gizmo** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **DynamicBoneSphereColliderGizmo** allows for interacting with [Dynamic Bone Sphere Colliders](https://wiki.resonite.com/Component:DynamicBoneSphereCollider "Component:DynamicBoneSphereCollider") via a [Sphere Gizmo](https://wiki.resonite.com/Component:SphereGizmo "Component:SphereGizmo"). these are usually created by activating the gizmo option using the context menu while having a slot with a [Dynamic Bone Sphere Collider](https://wiki.resonite.com/Component:DynamicBoneSphereCollider "Component:DynamicBoneSphereCollider") selected.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `_target` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [DynamicBoneSphereCollider](https://wiki.resonite.com/Component:DynamicBoneSphereCollider "Component:DynamicBoneSphereCollider") >** | The collider to make a visual/gizmo for. |
| `_sphereGizmo` | **[SphereGizmo](https://wiki.resonite.com/Component:SphereGizmo "Component:SphereGizmo")** | The gizmo being used to control `_target` through this component. |

Fields
Collapse

## Usage

## Examples

## See Also

- [Component:DynamicBoneSphereCollider](https://wiki.resonite.com/Component:DynamicBoneSphereCollider "Component:DynamicBoneSphereCollider")
- [Component:DynamicBoneChain](https://wiki.resonite.com/Component:DynamicBoneChain "Component:DynamicBoneChain")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:DynamicBoneSphereColliderGizmo&oldid=93832](https://wiki.resonite.com/index.php?title=Component:DynamicBoneSphereColliderGizmo&oldid=93832)"

Contents