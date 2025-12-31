# Component:SegmentMesh

> Source: https://wiki.resonite.com/Component:SegmentMesh

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:SegmentMesh&diff=98053) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/b/b9/SegmentMeshComponent.png/510px-SegmentMeshComponent.png)](https://wiki.resonite.com/File:SegmentMeshComponent.png) **Segment Mesh** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **SegmentMesh** component is an evolved form of [Component:SlotSegmentMesh](https://wiki.resonite.com/Component:SlotSegmentMesh "Component:SlotSegmentMesh") the behavior is identical, except when not provided slots it will use local coordinate points instead.

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
| `Radius` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The radius of the line from `PointA`/`SlotA` to `PointB`/`SlotB` |
| `PointA` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The starting point of the generated line in local space. |
| `PointB` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The ending point of the generated line in local space. |
| `SlotA` | _direct_ **[TransformRelayRef](https://wiki.resonite.com/index.php?title=Type:TransformRelayRef&action=edit&redlink=1 "Type:TransformRelayRef (page does not exist)")** | The starting point of the generated line. This will be used instead of `PointA` if provided. |
| `SlotB` | _direct_ **[TransformRelayRef](https://wiki.resonite.com/index.php?title=Type:TransformRelayRef&action=edit&redlink=1 "Type:TransformRelayRef (page does not exist)")** | The ending point of the generated line. This will be used instead of `PointB` if provided. |
| `Shading` | **[Shading](https://wiki.resonite.com/Type:Shading "Type:Shading")** | Whether to use different shading like smooth or flat. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `BakeMesh:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Bake meshes is a sync method that creates a static mesh component with this component, replaces all references to this component with the static mesh component, then deletes this component. |

Triggers
Collapse

## Usage

Attach to a slot and insert into a [Component:MeshRenderer](https://wiki.resonite.com/Component:MeshRenderer "Component:MeshRenderer") to see the geometry. Don't forget to use a [Material](https://wiki.resonite.com/Material "Material").

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Component:SlotSegmentMesh](https://wiki.resonite.com/Component:SlotSegmentMesh "Component:SlotSegmentMesh")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:SegmentMesh&oldid=98053](https://wiki.resonite.com/index.php?title=Component:SegmentMesh&oldid=98053)"

Contents