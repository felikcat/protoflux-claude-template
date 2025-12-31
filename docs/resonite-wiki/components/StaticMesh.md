# Component:StaticMesh

> Source: https://wiki.resonite.com/Component:StaticMesh

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:StaticMesh&diff=98426) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/6/6c/StaticMeshComponent.png/510px-StaticMeshComponent.png)](https://wiki.resonite.com/File:StaticMeshComponent.png) **Static Mesh** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **StaticMesh** component is used to load a static mesh asset from the Uri specified in \`URL\`

Generally, you will not need to use this component directly, as it is created automatically when importing a new mesh, or when baking a [Procedural Mesh](https://wiki.resonite.com/Category:Components:Assets:Procedural_Meshes "Category:Components:Assets:Procedural Meshes") using the Sync Method `BakeMesh()`

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `URL` | **[Uri](https://wiki.resonite.com/Type:Uri "Type:Uri")** | The Uri pointing to the .meshx asset to be loaded |
| `Readable` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this component's data can be read via protoflux. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| ``RecalculateNormals:Func`1<Task`1<Bool>>`` | **[Func\`1](https://wiki.resonite.com/Type:Func%601 "Type:Func`1") < [Task\`1](https://wiki.resonite.com/index.php?title=Type:Task%601&action=edit&redlink=1 "Type:Task`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >>** | X | Will recalculate all of the vertex normals on the mesh. |
| ``RecalculateNormalsMerged:Func`1<Task`1<Bool>>`` | **[Func\`1](https://wiki.resonite.com/Type:Func%601 "Type:Func`1") < [Task\`1](https://wiki.resonite.com/index.php?title=Type:Task%601&action=edit&redlink=1 "Type:Task`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >>** | X | Recalculates this meshes vertex normals which effects shading. |
| ``RecalculateTangentsSimple:Func`1<Task`1<Bool>>`` | **[Func\`1](https://wiki.resonite.com/Type:Func%601 "Type:Func`1") < [Task\`1](https://wiki.resonite.com/index.php?title=Type:Task%601&action=edit&redlink=1 "Type:Task`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >>** | X | Recalulates mesh tangents which affect shading. Simple mode. |
| ``RecalculateTangentsMikktspace:Func`1<Task`1<Bool>>`` | **[Func\`1](https://wiki.resonite.com/Type:Func%601 "Type:Func`1") < [Task\`1](https://wiki.resonite.com/index.php?title=Type:Task%601&action=edit&redlink=1 "Type:Task`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >>** | X | Recalcates mesh tangents which affect shading. This is Mikkspace which is defined by UnityEngine's definition. |
| ``RecalculateBlendshapeNormals:Func`1<Task`1<Bool>>`` | **[Func\`1](https://wiki.resonite.com/Type:Func%601 "Type:Func`1") < [Task\`1](https://wiki.resonite.com/index.php?title=Type:Task%601&action=edit&redlink=1 "Type:Task`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >>** | X | Recalculate the normals of blendshape data. |
| ``RecalculateBlendshapeNormalsMerged:Func`1<Task`1<Bool>>`` | **[Func\`1](https://wiki.resonite.com/Type:Func%601 "Type:Func`1") < [Task\`1](https://wiki.resonite.com/index.php?title=Type:Task%601&action=edit&redlink=1 "Type:Task`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >>** | X | Recalculate the normals of blendshape data. Merged mode. |
| ``RecalculateBlendshapeTangentsMikktspace:Func`1<Task`1<Bool>>`` | **[Func\`1](https://wiki.resonite.com/Type:Func%601 "Type:Func`1") < [Task\`1](https://wiki.resonite.com/index.php?title=Type:Task%601&action=edit&redlink=1 "Type:Task`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >>** | X | Recalculate the normals of blendshape data in Mikktspace. |
| ``FlipNormals:Func`1<Task`1<Bool>>`` | **[Func\`1](https://wiki.resonite.com/Type:Func%601 "Type:Func`1") < [Task\`1](https://wiki.resonite.com/index.php?title=Type:Task%601&action=edit&redlink=1 "Type:Task`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >>** | X | Flips the vertex normals of the mesh (used to fix issues with shadows being on the lit side of a mesh) |
| ``ReverseWinding:Func`1<Task`1<Bool>>`` | **[Func\`1](https://wiki.resonite.com/Type:Func%601 "Type:Func`1") < [Task\`1](https://wiki.resonite.com/index.php?title=Type:Task%601&action=edit&redlink=1 "Type:Task`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >>** | X | Reverses the vertex winding order of the mesh (used to fix issues where mesh is "inside out") |
| ``MakeDualSided:Func`1<Task`1<Bool>>`` | **[Func\`1](https://wiki.resonite.com/Type:Func%601 "Type:Func`1") < [Task\`1](https://wiki.resonite.com/index.php?title=Type:Task%601&action=edit&redlink=1 "Type:Task`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >>** | X | Duplicates all vertices on the mesh, but with an inverted winding, which allows it to be seen from both sides. |
| ``ConvertToFlatShading:Func`1<Task`1<Bool>>`` | **[Func\`1](https://wiki.resonite.com/Type:Func%601 "Type:Func`1") < [Task\`1](https://wiki.resonite.com/index.php?title=Type:Task%601&action=edit&redlink=1 "Type:Task`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >>** | X | Duplicates all shared vertices on the mesh, so that the vertex normals for a given face can be perpendicular, resulting in a faceted (or "flat") look. |
| ``MergeDoubles:Func`1<Task`1<Bool>>`` | **[Func\`1](https://wiki.resonite.com/Type:Func%601 "Type:Func`1") < [Task\`1](https://wiki.resonite.com/index.php?title=Type:Task%601&action=edit&redlink=1 "Type:Task`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >>** | X | Merges all the vertices in the exact same place on the mesh. |
| ``StripEmptyBlendshapes:Func`1<Task`1<Bool>>`` | **[Func\`1](https://wiki.resonite.com/Type:Func%601 "Type:Func`1") < [Task\`1](https://wiki.resonite.com/index.php?title=Type:Task%601&action=edit&redlink=1 "Type:Task`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >>** | X | Strips blendshapes from the mesh that don't move any vertices. |
| ``MergeBlendshapes:Func`1<Task`1<Bool>>`` | **[Func\`1](https://wiki.resonite.com/Type:Func%601 "Type:Func`1") < [Task\`1](https://wiki.resonite.com/index.php?title=Type:Task%601&action=edit&redlink=1 "Type:Task`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >>** | X | Merges the blendshapes and returns a task that will complete in the future with a boolean. |
| ``StripBlendshapeNormals:Func`1<Task`1<Bool>>`` | **[Func\`1](https://wiki.resonite.com/Type:Func%601 "Type:Func`1") < [Task\`1](https://wiki.resonite.com/index.php?title=Type:Task%601&action=edit&redlink=1 "Type:Task`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >>** | X | Gets rid of per shapekey normal data |
| ``StripBlendshapeTangents:Func`1<Task`1<Bool>>`` | **[Func\`1](https://wiki.resonite.com/Type:Func%601 "Type:Func`1") < [Task\`1](https://wiki.resonite.com/index.php?title=Type:Task%601&action=edit&redlink=1 "Type:Task`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >>** | X | Gets rid of per shapekey tangent data. |
| ``TrimBoneWeightCount:Func`2<Int, Task`1<Bool>>`` | **[Func\`2](https://wiki.resonite.com/Type:Func%602 "Type:Func`2") < [Int](https://wiki.resonite.com/Type:Int "Type:Int"), [Task\`1](https://wiki.resonite.com/index.php?title=Type:Task%601&action=edit&redlink=1 "Type:Task`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >>** | X | Reduces the amount of bones allowed to be weighted to a mesh per vertex. |
| ``ConvertToConvexHull:Func`1<Task`1<Bool>>`` | **[Func\`1](https://wiki.resonite.com/Type:Func%601 "Type:Func`1") < [Task\`1](https://wiki.resonite.com/index.php?title=Type:Task%601&action=edit&redlink=1 "Type:Task`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >>** | X | creates a Convex Hull Mesh from this mesh. Which a good analogy is wrapping the mesh in plastic wrap for a new shape. |
| ``ConvertToPointCloud:Func`1<Task`1<Bool>>`` | **[Func\`1](https://wiki.resonite.com/Type:Func%601 "Type:Func`1") < [Task\`1](https://wiki.resonite.com/index.php?title=Type:Task%601&action=edit&redlink=1 "Type:Task`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >>** | X | Creates a mesh that is a cloud of points using the vertices of this mesh. |
| ``TranslateUVs:Func`3<Float4, Float4, Task`1<Bool>>`` | **[Func\`3](https://wiki.resonite.com/Type:Func%603 "Type:Func`3") < [Float4](https://wiki.resonite.com/Type:Float4 "Type:Float4"), [Float4](https://wiki.resonite.com/Type:Float4 "Type:Float4"), [Task\`1](https://wiki.resonite.com/index.php?title=Type:Task%601&action=edit&redlink=1 "Type:Task`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >>** | X | Transforms the mesh UVs around. |
| `ResaveMesh:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Resaves the mesh recieved on the client to the cloud. can fix syncing issues with other users. |
| `RecalculateNormals:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Use above function instead. |
| `RecalculateNormalsMerged:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Use above function instead. |
| `RecalculateTangentsSimple:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Use above function instead. |
| `RecalculateTangentsMikk:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Use above function instead. |
| `RecalculateBlendshapeNormals:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Use above function instead. |
| `RecalculateBlendshapeNormalsMerged:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Use above function instead. |
| `RecalculateBlendshapeTangentsMikk:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Use above function instead. |
| `FlipNormals:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Use above function instead. |
| `ReverseWinding:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Use above function instead. |
| `MakeDualSided:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Use above function instead. |
| `ConvertToFlatShading:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Use above function instead. |
| `MergeDoubles:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Use above function instead. |
| `StripEmptyBlendshapes:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Use above function instead. |
| `MergeBlendshapes:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Use above function instead. |
| `StripBlendshapeNormals:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Use above function instead. |
| `StripBlendshapeTangents:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Use above function instead. |
| ``TrimBoneWeightCount:ButtonEventHandler`1<Int>`` | **[ButtonEventHandler\`1](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler%601&action=edit&redlink=1 "Type:ButtonEventHandler`1 (page does not exist)") < [Int](https://wiki.resonite.com/Type:Int "Type:Int") >** | ✓ | Use above function instead. |
| `ConvertToConvexHull:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Converts the mesh to a convex hull. |
| `ConvertToPointCloud:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Converts the mesh to a point cloud. |
| `GetBoneList:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Creates a dialog that shows the bone list. |
| `GetBoneData:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Creates a dialog that shows the bone data. |
| ``ScaleUVs:ButtonEventHandler`1<FloatTextEditorParser>`` | **[ButtonEventHandler\`1](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler%601&action=edit&redlink=1 "Type:ButtonEventHandler`1 (page does not exist)") < [FloatTextEditorParser](https://wiki.resonite.com/Component:FloatTextEditorParser "Component:FloatTextEditorParser") >** | ✓ | Scales the UVs by the recieved size. |

Triggers
Collapse

## Usage

Attach to a slot, provide a `URL` and insert into a [Component:SkinnedMeshRenderer](https://wiki.resonite.com/Component:SkinnedMeshRenderer "Component:SkinnedMeshRenderer") or [Component:MeshRenderer](https://wiki.resonite.com/Component:MeshRenderer "Component:MeshRenderer"). Don't forget the [Material](https://wiki.resonite.com/Material "Material")(s).

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:StaticMesh&oldid=98426](https://wiki.resonite.com/index.php?title=Component:StaticMesh&oldid=98426)"

Contents