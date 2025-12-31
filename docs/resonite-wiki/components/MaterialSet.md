# Component:MaterialSet

> Source: https://wiki.resonite.com/Component:MaterialSet

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/6/61/MaterialSetComponent.png/510px-MaterialSetComponent.png)](https://wiki.resonite.com/File:MaterialSetComponent.png) **Material Set** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

Material set allows for switching the list of materials being used on a mesh dynamically at any given moment. It also allows for lengthening or shortening the list in real time, which can be used to [material stack (things to avoid)](https://wiki.resonite.com/Things_to_Avoid#Material_%22Stacking%22 "Things to Avoid").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `ActiveSetIndex` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The index into the Sets list of the materials to apply to the target renderer. |
| `Target` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[SyncAssetList\`1](https://wiki.resonite.com/Type:SyncAssetList%601 "Type:SyncAssetList`1") < [Material](https://wiki.resonite.com/Type:Material "Type:Material") >** | The list of materials in a renderer to swap out. |
| `Sets` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[SyncAssetList\`1](https://wiki.resonite.com/Type:SyncAssetList%601 "Type:SyncAssetList`1") < [Material](https://wiki.resonite.com/Type:Material "Type:Material") >** | The list of lists of materials in a renderer to swap out. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `OnSetupFromMeshRenderer:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the setup from mesh renderer button is touched. |

Triggers
Collapse

## Usage

Attach this component to the same slot as a [Mesh Renderer](https://wiki.resonite.com/Component:MeshRenderer "Component:MeshRenderer") or a [Skinned Mesh Renderer](https://wiki.resonite.com/Component:SkinnedMeshRenderer "Component:SkinnedMeshRenderer") and hit the `Setup From Mesh Renderer()` [sync delegate](https://wiki.resonite.com/Sync_Delegate "Sync Delegate") to attach it to the material list. Next add a list ( [SyncAssetList\`1](https://wiki.resonite.com/Type:SyncAssetList%601 "Type:SyncAssetList`1") < [Material](https://wiki.resonite.com/Type:Material "Type:Material") >) of each material list to `Sets` you want to switch between. Lastly use `ActiveSetIndex` to switch between each list in `Sets` for `Target`.

## Examples

Can be used to switch a material set on an avatar to make them change material types ( [toon](https://wiki.resonite.com/Component:XiexeToonMaterial "Component:XiexeToonMaterial") to [pbs metallic](https://wiki.resonite.com/Component:PBS_Metallic "Component:PBS Metallic")) or from active camo to not active camo, etc.

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:MaterialSet&oldid=99069](https://wiki.resonite.com/index.php?title=Component:MaterialSet&oldid=99069)"

Contents