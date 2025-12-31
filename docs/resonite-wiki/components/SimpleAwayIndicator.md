# Component:SimpleAwayIndicator

> Source: https://wiki.resonite.com/Component:SimpleAwayIndicator

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:SimpleAwayIndicator&diff=99192) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/4/4a/SimpleAwayIndicatorComponent.png/510px-SimpleAwayIndicatorComponent.png)](https://wiki.resonite.com/File:SimpleAwayIndicatorComponent.png) **SimpleAwayIndicator** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **SimpleAwayIndicator** indicates when a user doesn't have the session focused by temporarily replacing the [materials](https://wiki.resonite.com/Material "Material") of a [MeshRenderer](https://wiki.resonite.com/Component:MeshRenderer "Component:MeshRenderer") with the specified _Away Material_.

Usually found on the body [slot](https://wiki.resonite.com/Slot "Slot") of an [avatar](https://wiki.resonite.com/Avatar "Avatar") (but can be put anywhere in the [world](https://wiki.resonite.com/World "World")), this just needs a [reference](https://wiki.resonite.com/Reference_Type "Reference Type") to the [MeshRenderer](https://wiki.resonite.com/Component:MeshRenderer "Component:MeshRenderer") or [SkinnedMeshRenderer](https://wiki.resonite.com/Component:SkinnedMeshRenderer "Component:SkinnedMeshRenderer") components to work.

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `User` | **[User](https://wiki.resonite.com/Type:User "Type:User")** | User whose away state will be watched. _On avatars, may be set by an [AvatarUserReferenceAssigner](https://wiki.resonite.com/Component:AvatarUserReferenceAssigner "Component:AvatarUserReferenceAssigner") component._ |
| `AwayMaterial` | **[Material](https://wiki.resonite.com/Type:Material "Type:Material")** | Material to display when the user is away. |
| `Renderer` | **[MeshRenderer](https://wiki.resonite.com/Component:MeshRenderer "Component:MeshRenderer")** | Mesh renderer component whose materials should be replaced |
| `_oldMaterials` | _[list](https://wiki.resonite.com/Type:SyncAssetList%601 "Type:SyncAssetList`1")_ of **[Material](https://wiki.resonite.com/Type:Material "Type:Material")** | Backup of the renderer's original material list. _Written automatically when "Away" state is triggered._ |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `SetAway:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Stores the renderer's material list in `_oldMaterials` and replaces them with the `AwayMaterial`. |
| `Restore:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Restores the renderer's materials from `_oldMaterials`. |
| `OnTestAway:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Stores the renderer's material list in `_oldMaterials` and replaces them with the `AwayMaterial`. |
| `OnTestRestore:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Restores the renderer's materials from `_oldMaterials`. |

Triggers
Collapse

## Usage

This is used to make a customized or fancier way of stating that you are focused away into another [world](https://wiki.resonite.com/World "World").

## Examples

Used on avatar meshes so they show an away Material when the user is away.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:SimpleAwayIndicator&oldid=99192](https://wiki.resonite.com/index.php?title=Component:SimpleAwayIndicator&oldid=99192)"

Contents