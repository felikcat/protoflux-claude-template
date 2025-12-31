# Component:RampMesh

> Source: https://wiki.resonite.com/Component:RampMesh

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:RampMesh&diff=98034) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/2/28/RampMeshComponent.png/510px-RampMeshComponent.png)](https://wiki.resonite.com/File:RampMeshComponent.png) **Ramp Mesh** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **RampMesh** component procedurally generates mesh data for a ramp shaped mesh.

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
| `Length` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How long the ramp is |
| `Height` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The height of the ramp |
| `Width` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How wide the ramp is |
| `UVScale` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | Changes the UV scale of the procedural mesh. |

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

Car ramps, mobility ramps, etc.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:RampMesh&oldid=98034](https://wiki.resonite.com/index.php?title=Component:RampMesh&oldid=98034)"

Contents