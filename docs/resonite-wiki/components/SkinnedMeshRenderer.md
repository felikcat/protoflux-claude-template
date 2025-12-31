# Component:SkinnedMeshRenderer

> Source: https://wiki.resonite.com/Component:SkinnedMeshRenderer

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/d/d7/SkinnedMeshRendererComponent.png/510px-SkinnedMeshRendererComponent.png)](https://wiki.resonite.com/File:SkinnedMeshRendererComponent.png) **SkinnedMeshRenderer** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **SkinnedMeshRenderer** component is used for rendering animated/dynamic 3D meshes in the world, and applying materials to that mesh.

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
| `BoundsComputeMethod` | **[SkinnedBounds](https://wiki.resonite.com/Type:SkinnedBounds "Type:SkinnedBounds")** | How the bounds of this mesh will be calculated. Should be left as _Static_ if possible, for performance reasons. |
| `ProxyBoundsSource` | **SkinnedMeshRenderer** | A SkinnedMeshRenderer to use the `ExplicitLocalBounds` of rather than the `ExplicitLocalBounds` on this component. |
| `ExplicitLocalBounds` | **[BoundingBox](https://wiki.resonite.com/Type:BoundingBox "Type:BoundingBox")** | A box that within view will render the mesh, and when out of view will cull the mesh and stop rendering it. Is used when `ProxyBoundsSource` is null. |
| `Bones` | _[list](https://wiki.resonite.com/Type:SyncRefList%601 "Type:SyncRefList`1")_ of **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | _Automatically Assigned_ — List of bones present in this mesh |
| `BlendShapeWeights` | _direct_ **[SyncFieldList\`1](https://wiki.resonite.com/Type:SyncFieldList%601 "Type:SyncFieldList`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | _Automatically Assigned_ — List of blendshapes present in this mesh, and their respective weights. |

Fields
Collapse

### Sync delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| ``SplitBlenshapeAlongAxis:Func`7<Int, Axis3D, Float, Float, String, String, Task`1<Bool>>`` | **[Func\`7](https://wiki.resonite.com/index.php?title=Type:Func%607&action=edit&redlink=1 "Type:Func`7 (page does not exist)") < [Int](https://wiki.resonite.com/Type:Int "Type:Int"), [Axis3D](https://wiki.resonite.com/index.php?title=Type:Axis3D&action=edit&redlink=1 "Type:Axis3D (page does not exist)"), [Float](https://wiki.resonite.com/Type:Float "Type:Float"), [Float](https://wiki.resonite.com/Type:Float "Type:Float"), [String](https://wiki.resonite.com/Type:String "Type:String"), [String](https://wiki.resonite.com/Type:String "Type:String"), [Task\`1](https://wiki.resonite.com/index.php?title=Type:Task%601&action=edit&redlink=1 "Type:Task`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >>** | X | Splits a blendshape along a given axis, and returns a task representing if the operation is done yet. |
| ``BakeBlendshape:Func`2<Int, Task`1<Bool>>`` | **[Func\`2](https://wiki.resonite.com/Type:Func%602 "Type:Func`2") < [Int](https://wiki.resonite.com/Type:Int "Type:Int"), [Task\`1](https://wiki.resonite.com/index.php?title=Type:Task%601&action=edit&redlink=1 "Type:Task`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >>** | X | bakes a blendshape to make it part of the mesh rest state, and returns a task representing if the operation is done yet. |
| ``RemoveBlendshape:Func`2<Int, Task`1<Bool>>`` | **[Func\`2](https://wiki.resonite.com/Type:Func%602 "Type:Func`2") < [Int](https://wiki.resonite.com/Type:Int "Type:Int"), [Task\`1](https://wiki.resonite.com/index.php?title=Type:Task%601&action=edit&redlink=1 "Type:Task`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >>** | X | removes a blendshape from the mesh, and returns a task representing if the operation is done yet. |
| `VisualizeApproximateBoneBounds:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Makes a series of boxes showing the bounds of the bones in the mesh. |
| `VisualizeBoneBounds:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Makes a series of boxes showing the bounds of the bones in the mesh. |
| `ClearBoundsVisuals:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | clears bound visuals. |
| `SeparateOutBlendshapes:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Separates out the blendshape affected mesh parts from the non blendshape affected mesh parts. |
| `StripEmptyBlendshapes:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Removes blendshapes that don't change anything. |
| `BakeNonDrivenBlendshapes:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Bakes all blendshapes on the mesh that aren't driven based on their current value, making it part of the rest state. |
| `BakeToStaticMesh:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Bakes the mesh and makes it a static mesh instead. |
| `MergeBlendshapes:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Combine all blendshapes in to one blendshape, which interpolates between the source blendshapes like a playback timeline. |
| `StripEmptyBones:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Gets rid of bones that have no vertices assigned to them. |
| `ComputeExplicitBoundsFromPose:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Computes the explicit bounds property for the skinned mesh renderer component based on it's current pose of it's bones. |
| `ExtendExplicitBoundsFromPose:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | extends the bounds of the explicit bounds property for the skinned mesh renderer component based on it's current pose of it's bones. |
| `SortBlendshapesByName:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Sorts blendshapes by name in alphabetical order. |
| `SortBlendshapesByNameLength:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Sorts blendshapes by how many characters are in a given blendshape name. |
| `SplitSubmeshes:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Will split this mesh into additional submeshes, each having only one material |
| `MergeByMaterial:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Will merge all submeshes that use the same material |

Triggers
Collapse

## Usage

While it _can_ be used for rendering static meshes, it is **not recommended** as there is a slight performance penalty for using SkinnedMeshRenderer, even if the animation features aren't used — Please try to use [MeshRenderer](https://wiki.resonite.com/MeshRenderer_(Component) "MeshRenderer (Component)") where possible.

## Examples

## See also

- [Component:MeshRenderer](https://wiki.resonite.com/Component:MeshRenderer "Component:MeshRenderer")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:SkinnedMeshRenderer&oldid=108406](https://wiki.resonite.com/index.php?title=Component:SkinnedMeshRenderer&oldid=108406)"

Contents