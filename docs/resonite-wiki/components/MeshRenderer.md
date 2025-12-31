# Component:MeshRenderer

> Source: https://wiki.resonite.com/Component:MeshRenderer

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/d/d1/MeshRendererComponent.png/510px-MeshRendererComponent.png)](https://wiki.resonite.com/File:MeshRendererComponent.png) **MeshRenderer** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **MeshRenderer** component is used for rendering static 3D meshes in the world, and applying materials to that mesh.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Mesh` | **[Mesh](https://wiki.resonite.com/Type:Mesh "Type:Mesh")** | The mesh to be rendered. Can be a [StaticMesh](https://wiki.resonite.com/StaticMesh_(Component) "StaticMesh (Component)") or a [Procedural Mesh](https://wiki.resonite.com/Category:Components:Assets:Procedural_Meshes "Category:Components:Assets:Procedural Meshes") |
| `Materials` | _[list](https://wiki.resonite.com/Type:SyncAssetList%601 "Type:SyncAssetList`1")_ of **[Material](https://wiki.resonite.com/Type:Material "Type:Material")** | A list of materials to be applied to the mesh |
| `MaterialPropertyBlocks` | _[list](https://wiki.resonite.com/Type:SyncAssetList%601 "Type:SyncAssetList`1")_ of **[MaterialPropertyBlock](https://wiki.resonite.com/index.php?title=Type:MaterialPropertyBlock&action=edit&redlink=1 "Type:MaterialPropertyBlock (page does not exist)")** | A list of material property blocks to apply to the materials on this mesh. Usually used for performance reasons where using multiple similar materials would take more resources. |
| `ShadowCastMode` | **[ShadowCastMode](https://wiki.resonite.com/Type:ShadowCastMode "Type:ShadowCastMode")** | How this object will cast shadows onto the world, or if it _only_ draws a shadow. |
| `MotionVectorMode` | **[MotionVectorMode](https://wiki.resonite.com/Type:MotionVectorMode "Type:MotionVectorMode")** | See Motion vector mode. |
| `SortingOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Whether to render this before or after other renderers with geometry in the same location. |

Fields
Collapse

## Sync delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `SplitSubmeshes:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Will split this mesh into additional submeshes, each having only one material. |
| `MergeByMaterial:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Will merge all submeshes that use the same material. |
| `SplitSubmeshes:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the split submeshes button is touched. |
| `MergeByMaterial:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the merge by material button is touched. |

Triggers
Collapse

## Usage

## Examples

## See also

- [Component:SkinnedMeshRenderer](https://wiki.resonite.com/Component:SkinnedMeshRenderer "Component:SkinnedMeshRenderer")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:MeshRenderer&oldid=108401](https://wiki.resonite.com/index.php?title=Component:MeshRenderer&oldid=108401)"

Contents