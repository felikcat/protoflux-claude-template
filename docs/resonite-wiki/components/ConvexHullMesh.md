# Component:ConvexHullMesh

> Source: https://wiki.resonite.com/Component:ConvexHullMesh

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/6/69/ConvexHullMeshComponent.png/510px-ConvexHullMeshComponent.png)](https://wiki.resonite.com/File:ConvexHullMeshComponent.png) **Convex Hull Mesh** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ConvexHullMesh** component is used to generate a Convex Hull Mesh using a series of `Points` to wrap around.

The `Points` field is not editable currently without [Mods](https://wiki.resonite.com/Mods "Mods").

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `HighPriorityIntegration` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | If true, integrating this asset (e.g. processing procedural assets) gets higher priority than assets with this flag off. An example is user laser procedural meshes. |
| `OverrideBoundingBox` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Force the bounding box calculated from this component to use `OverridenBoundingBox` instead of calculating when requested. |
| `OverridenBoundingBox` | **[BoundingBox](https://wiki.resonite.com/Type:BoundingBox "Type:BoundingBox")** | the bounding box this component should say it has when `OverrideBoundingBox` is enabled. Useful for bounding box calculations with Flux, or changing the selection box for this component when rendered. |
| `Profile` | **[ColorProfile](https://wiki.resonite.com/Type:ColorProfile "Type:ColorProfile")** | The profile that the vertex colors for this mesh should be displayed in. |
| `Points` | _[array](https://wiki.resonite.com/Type:SyncArray%601 "Type:SyncArray`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The points in local space this mesh is trying to shrink wrap around. |
| `FlatShading` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the geometry should be not smooth. |
| `MinVertexDistance` | **[Double](https://wiki.resonite.com/Type:Double "Type:Double")** | the distance by minimum 2 `Points` can be before they're automatically merged. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `BakeMesh:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Bake meshes is a sync method that creates a static mesh component with this component, replaces all references to this component with the static mesh component, then deletes this component. |

Triggers
Collapse

## Usage

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ConvexHullMesh&oldid=97908](https://wiki.resonite.com/index.php?title=Component:ConvexHullMesh&oldid=97908)"

Contents