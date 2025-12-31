# Component:TubeBoxMesh

> Source: https://wiki.resonite.com/Component:TubeBoxMesh

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:TubeBoxMesh&diff=98099) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/d/d4/TubeBoxMeshComponent.png/510px-TubeBoxMeshComponent.png)](https://wiki.resonite.com/File:TubeBoxMeshComponent.png) **Tube Box Mesh** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **TubeBoxMesh** component is used to generate geometry that is used with a [Component:MeshRenderer](https://wiki.resonite.com/Component:MeshRenderer "Component:MeshRenderer").

_This article or section is a stub. You can help the Resonite wiki by expanding it._

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
| `Size` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | How big the box is. |
| `TubeRadius` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | how big the tube is |
| `SegmentPoints` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The divisions in geometry/edges in the tube's circular direction. |
| `UVScale` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The scale of material detail on the mesh. |
| `UVOffset` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The offset of material detail on the mesh. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `BakeMesh:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Bake meshes is a sync method that creates a static mesh component with this component, replaces all references to this component with the static mesh component, then deletes this component. |

Triggers
Collapse

## Usage

Attach to a slot and insert into a [Component:MeshRenderer](https://wiki.resonite.com/Component:MeshRenderer "Component:MeshRenderer") to view the geometry. Don't forget to use a [Material](https://wiki.resonite.com/Material "Material").

## Examples

[![An example of what TubeBoxMesh looks like](https://wiki.resonite.com/images/thumb/f/fd/TubeBoxMeshExample.jpg/800px-TubeBoxMeshExample.jpg)](https://wiki.resonite.com/File:TubeBoxMeshExample.jpg "An example of what TubeBoxMesh looks like")

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:TubeBoxMesh&oldid=98099](https://wiki.resonite.com/index.php?title=Component:TubeBoxMesh&oldid=98099)"

Contents