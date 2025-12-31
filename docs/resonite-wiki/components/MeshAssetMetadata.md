# Component:MeshAssetMetadata

> Source: https://wiki.resonite.com/Component:MeshAssetMetadata

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:MeshAssetMetadata&diff=94940) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/1/15/MeshAssetMetadataComponent.png/510px-MeshAssetMetadataComponent.png)](https://wiki.resonite.com/File:MeshAssetMetadataComponent.png) **Mesh Asset Metadata** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **MeshAssetMetadata** component gives info about the data on a mesh component.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Mesh` | **[Mesh](https://wiki.resonite.com/Type:Mesh "Type:Mesh")** | The mesh to get meta data on. |
| `VertexCount` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The amount of vertices in `Mesh`. |
| `TriangleCount` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The amount of triangles in `Mesh`. |
| `PointCount` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | the amount of vertices with no connected faces in `Mesh`. |
| `SubmeshCount` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | How many sub meshes are in the main `Mesh`. |
| `BoneCount` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The amount of bones in `Mesh`. |
| `BlendshapeCount` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The amount of blendshapes in `Mesh`. |
| `HasNormals` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether `Mesh` has normal data. |
| `HasTangents` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether `Mesh` has tangent data. |
| `HasVertexColors` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether `Mesh` has vertex color data. |
| `HasUV0s` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether `Mesh` has data for the first UV map. |
| `HasUV1s` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether `Mesh` has data for the second UV map. |
| `HasUV2s` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether `Mesh` has data for the third UV map. |
| `HasUV3s` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether `Mesh` has data for the fourth UV map. |

Fields
Collapse

## Usage

Attach to a slot and provide a Mesh to `Mesh` to make the component output data.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:MeshAssetMetadata&oldid=94940](https://wiki.resonite.com/index.php?title=Component:MeshAssetMetadata&oldid=94940)"

Contents