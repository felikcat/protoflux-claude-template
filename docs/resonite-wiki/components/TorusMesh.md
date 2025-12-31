# Component:TorusMesh

> Source: https://wiki.resonite.com/Component:TorusMesh

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:TorusMesh&diff=98093) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/1/10/TorusMeshComponent.png/510px-TorusMeshComponent.png)](https://wiki.resonite.com/File:TorusMeshComponent.png) **Torus Mesh** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **TorusMesh** component generates procedural geometry that is used with [Component:MeshRenderer](https://wiki.resonite.com/Component:MeshRenderer "Component:MeshRenderer").

This mesh resembles a Donut.

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
| `MinorSegments` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The amount of detail/cuts along the circle of the torus. Making this 4 will make the torus a square instead of a circle shape. |
| `MajorSegments` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The amount of detail/cuts going around and through the center along the outside and inside. |
| `MajorRadius` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The size of the torus |
| `MinorRadius` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | the fatness/thickness of the torus. If this is too big than the hole in the center will seal up. |
| `UVScale` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | the scale of the material detail on the surface of the torus. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `BakeMesh:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Bake meshes is a sync method that creates a static mesh component with this component, replaces all references to this component with the static mesh component, then deletes this component. |

Triggers
Collapse

## Usage

Attach to a slot and insert this component into a [Component:MeshRenderer](https://wiki.resonite.com/Component:MeshRenderer "Component:MeshRenderer") to view its geometry. Don't forget to add a [Material](https://wiki.resonite.com/Material "Material")

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:TorusMesh&oldid=98093](https://wiki.resonite.com/index.php?title=Component:TorusMesh&oldid=98093)"

Contents