# Component:MaterialApplyPolicy

> Source: https://wiki.resonite.com/Component:MaterialApplyPolicy

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:MaterialApplyPolicy&oldid=95135&diff=113865) which are not marked for translation.

Other languages:

- English
- [日本語](https://wiki.resonite.com/Component:MaterialApplyPolicy/ja "コンポーネント:MaterialApplyPolicy (100% translated)")

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/c/c5/MaterialApplyPolicyComponent.png/510px-MaterialApplyPolicyComponent.png)](https://wiki.resonite.com/File:MaterialApplyPolicyComponent.png) **MaterialApplyPolicy** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **MaterialApplyPolicy** component allows for controlling whether a [Material Tool](https://wiki.resonite.com/Material_Tool "Material Tool") is able to apply a [material](https://wiki.resonite.com/Material "Material") to the [slot](https://wiki.resonite.com/Slot "Slot") hierarchy [tagged](https://wiki.resonite.com/Tag "Tag") with this component onto its [SkinnedMeshRenderer](https://wiki.resonite.com/Component:SkinnedMeshRenderer "Component:SkinnedMeshRenderer")/ [MeshRenderer](https://wiki.resonite.com/Component:MeshRenderer "Component:MeshRenderer") components.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `CanApply` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Setting this to false will prevent the [Material Tool](https://wiki.resonite.com/Material_Tool "Material Tool") from applying materials to any [SkinnedMeshRenderer](https://wiki.resonite.com/Component:SkinnedMeshRenderer "Component:SkinnedMeshRenderer")/ [MeshRenderer](https://wiki.resonite.com/Component:MeshRenderer "Component:MeshRenderer") components in the slot or child slots. |

Fields
Collapse

## Usage

When this component is added to a [Slot](https://wiki.resonite.com/Slot "Slot") with a [SkinnedMeshRenderer](https://wiki.resonite.com/Component:SkinnedMeshRenderer "Component:SkinnedMeshRenderer") or [MeshRenderer](https://wiki.resonite.com/Component:MeshRenderer "Component:MeshRenderer") attached, it allows one to limit the effects of the [Material Tool](https://wiki.resonite.com/Material_Tool "Material Tool").

## Examples

On an avatar, you can try adding this component to the root of the avatar, making sure the avatar has a [Component:ObjectRoot](https://wiki.resonite.com/Component:ObjectRoot "Component:ObjectRoot"), and set `CanApply` to false. Doing this will ensure that the avatar's material cannot be changed by the Material Tool.

Adding this component to the Slot of a MeshRender and setting `CanApply` to true can allow one to explicitly change the material in specific places on small objects.

## See Also

- [MeshRenderer](https://wiki.resonite.com/Components:MeshRenderer "Components:MeshRenderer")
- [SkinnedMeshRenderer](https://wiki.resonite.com/Components:SkinnedMeshRenderer "Components:SkinnedMeshRenderer")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:MaterialApplyPolicy&oldid=113865](https://wiki.resonite.com/index.php?title=Component:MaterialApplyPolicy&oldid=113865)"

Contents