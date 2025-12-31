# Component:SlotSegmentMesh

> Source: https://wiki.resonite.com/Component:SlotSegmentMesh

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:SlotSegmentMesh&diff=98071) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/9/9d/SlotSegmentMeshComponent.png/510px-SlotSegmentMeshComponent.png)](https://wiki.resonite.com/File:SlotSegmentMeshComponent.png) **Slot Segment Mesh** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **SlotSegmentMesh** component generates mesh data of a line between `PointA` and `PointB`. This is to be used with a [Component:MeshRenderer](https://wiki.resonite.com/Component:MeshRenderer "Component:MeshRenderer").

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
| `Radius` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The radius of the line from `PointA` to `PointB` |
| `PointA` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The starting point of the generated line. |
| `PointB` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The ending point of the generated line. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `BakeMesh:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Bake meshes is a sync method that creates a static mesh component with this component, replaces all references to this component with the static mesh component, then deletes this component. |

Triggers
Collapse

## Usage

Attach to a slot and then insert into a [Component:MeshRenderer](https://wiki.resonite.com/Component:MeshRenderer "Component:MeshRenderer"). Don't forget to use a [Material](https://wiki.resonite.com/Material "Material").

## Examples

## See Also

- [Component:SegmentMesh](https://wiki.resonite.com/Component:SegmentMesh "Component:SegmentMesh")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:SlotSegmentMesh&oldid=98071](https://wiki.resonite.com/index.php?title=Component:SlotSegmentMesh&oldid=98071)"

Contents