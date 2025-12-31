# Component:TriangleMesh

> Source: https://wiki.resonite.com/Component:TriangleMesh

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:TriangleMesh&diff=98097) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/a/a0/TriangleMeshComponent.png/510px-TriangleMeshComponent.png)](https://wiki.resonite.com/File:TriangleMeshComponent.png) **Triangle Mesh** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **TriangeMesh** component is used to generate mesh data which is a triangle for use with a [Component:MeshRenderer](https://wiki.resonite.com/Component:MeshRenderer "Component:MeshRenderer").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `HighPriorityIntegration` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | If true, integrating this asset (e.g. processing procedural assets) gets higher priority than assets with this flag off. An example is user laser procedural meshes. |
| `OverrideBoundingBox` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Force the bounding box calculated from this component to use `OverridenBoundingBox` instead of calculating when requested. |
| `OverridenBoundingBox` | **[BoundingBox](https://wiki.resonite.com/Type:BoundingBox "Type:BoundingBox")** | the bounding box this component should say it has when `OverrideBoundingBox` is enabled. Useful for bounding box calculations with Flux, or changing the selection box for this component when rendered. |
| `Profile` | **[ColorProfile](https://wiki.resonite.com/Type:ColorProfile "Type:ColorProfile")** | The profile that the vertex colors for this mesh should be displayed in. |
| `Vertex0` | _direct_ **[TriangleMesh.Vertex](https://wiki.resonite.com/Component:TriangleMesh#Vertex)** | The first vertex point of the triangle. |
| `Vertex1` | _direct_ **[TriangleMesh.Vertex](https://wiki.resonite.com/Component:TriangleMesh#Vertex)** | The second vertex point of the triangle. |
| `Vertex2` | _direct_ **[TriangleMesh.Vertex](https://wiki.resonite.com/Component:TriangleMesh#Vertex)** | The third vertex point of the triangle. |
| `AutoNormals` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | whether to automatically generate the triangle normals |
| `AutoTangents` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | whether to automatically generate the triangle tangents |
| `DualSided` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | whether to make this visible from the back. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `BakeMesh:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Bake meshes is a sync method that creates a static mesh component with this component, replaces all references to this component with the static mesh component, then deletes this component. |

Triggers
Collapse

## Vertex

| Name | Type | Description |
| --- | --- | --- |
| `Position` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The position of the triangle vertex in global space. |
| `UV0` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The UV position of the vertex on the 0th uv map. |
| `UV1` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The UV position of the vertex on the 1st uv map. |
| `UV2` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The UV position of the vertex on the 2nd uv map. |
| `UV3` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The UV position of the vertex on the 3rd uv map. |
| `Color` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The vertex color of this vertex. |
| `Normal` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | the normal direction of this vertex |
| `Tangent` | **[Float4](https://wiki.resonite.com/Type:Float4 "Type:Float4")** | the tangent direction of this vertex. |

Fields

## Usage

Attach to a slot and insert the component into a [Component:MeshRenderer](https://wiki.resonite.com/Component:MeshRenderer "Component:MeshRenderer") to see what the mesh looks like. Don't forget to add a [Material](https://wiki.resonite.com/Material "Material").

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

(Maybe show [Magglor's](https://wiki.resonite.com/index.php?title=User:Magglor&action=edit&redlink=1 "User:Magglor (page does not exist)") triangle tool? And maybe one other example?)

## See Also

- [Component:StaticMesh](https://wiki.resonite.com/Component:StaticMesh "Component:StaticMesh")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:TriangleMesh&oldid=98097](https://wiki.resonite.com/index.php?title=Component:TriangleMesh&oldid=98097)"

Contents