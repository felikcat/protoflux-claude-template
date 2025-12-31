# Component:MultiSegmentMesh

> Source: https://wiki.resonite.com/Component:MultiSegmentMesh

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:MultiSegmentMesh&diff=99073) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/1/1c/MultiSegmentMeshComponent.png/510px-MultiSegmentMeshComponent.png)](https://wiki.resonite.com/File:MultiSegmentMeshComponent.png) **Multi Segment Mesh** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

Multi line segment mesh is a component that generates mesh data for use with a [SkinnedMeshRenderer](https://wiki.resonite.com/Component:SkinnedMeshRenderer "Component:SkinnedMeshRenderer"). It uses a list of [lines](https://wiki.resonite.com/Component:MultiSegmentMesh#SegmentInfo) to generate lines of geometry with varying thickness.

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
| `Sides` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | how many faces around each line (circle wise) that the lines have. |
| `FlipNormalDirection` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Flips the normals on the generated mesh data. |
| `Segments` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[MultiSegmentMesh.SegmentInfo](https://wiki.resonite.com/Component:MultiSegmentMesh#SegmentInfo)** | Different lines that make up the mesh. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `BakeMesh:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Bake meshes is a sync method that creates a static mesh component with this component, replaces all references to this component with the static mesh component, then deletes this component. |

Triggers
Collapse

## Usage

## SegmentInfo

| Name | Type | Description |
| --- | --- | --- |
| `Radius` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | how thick the line is in local space |
| `PointA` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The position of the start of the line in local space |
| `PointB` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The position of the end of the line in local space |

Fields

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:MultiSegmentMesh&oldid=99073](https://wiki.resonite.com/index.php?title=Component:MultiSegmentMesh&oldid=99073)"

Contents