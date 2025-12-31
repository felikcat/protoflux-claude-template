# Component:AvatarUserMeshHider

> Source: https://wiki.resonite.com/Component:AvatarUserMeshHider

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:AvatarUserMeshHider&diff=97400) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/b/bc/AvatarUserMeshHiderComponent.png/510px-AvatarUserMeshHiderComponent.png)](https://wiki.resonite.com/File:AvatarUserMeshHiderComponent.png) **AvatarUserMeshHider** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **AvatarUserMeshHider** component makes non Skinned meshes invisible or only cast shadows according to the active user's perspective. It does this by making value User overrides for all MeshRenderers except for those in `Exclude`. It restores the fields back to normal after dequipping.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Method` | **[AvatarUserMeshHider.HideMethod](https://wiki.resonite.com/Component:AvatarUserMeshHider#HideMethod)** | How to hide the meshes for the active user under the avatar. |
| `Exclude` | _[list](https://wiki.resonite.com/Type:SyncRefList%601 "Type:SyncRefList`1")_ of **[MeshRenderer](https://wiki.resonite.com/Component:MeshRenderer "Component:MeshRenderer")** | Which meshes to not hide for the active user. |

Fields
Collapse

## HideMethod

| Name | Value | Description |
| --- | --- | --- |
| `ShadowOnly` | 0 | Hide the meshes by value user overriding them to Shadow Only for the active user |
| `Deactivate` | 1 | Hide the meshes by value user overriding their active field to false only for the active user. |

Values

## Usage

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AvatarUserMeshHider&oldid=97400](https://wiki.resonite.com/index.php?title=Component:AvatarUserMeshHider&oldid=97400)"

Contents