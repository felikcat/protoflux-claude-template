# Component:BevelBoxMesh

> Source: https://wiki.resonite.com/Component:BevelBoxMesh

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:BevelBoxMesh&diff=97870) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/7/78/BevelBoxMeshComponent.png/510px-BevelBoxMeshComponent.png)](https://wiki.resonite.com/File:BevelBoxMeshComponent.png) **Bevel Box Mesh** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The BevelBoxMesh component can be placed in a [MeshRenderer](https://wiki.resonite.com/Component:MeshRenderer "Component:MeshRenderer") to create a box with beveled edges.

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
| `Size` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The 3-Dimentional scale of the mesh. |
| `Bevel` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Size of the rounded edges. |
| `UVScale` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The inverse of the size the material should appear on the surface as. |
| `ScaleUVWithSize` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Change uv scale visually with the value of `Size` |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `BakeMesh:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Bake meshes is a sync method that creates a static mesh component with this component, replaces all references to this component with the static mesh component, then deletes this component. |

Triggers
Collapse

## Usage

Attach to a slot, and assign to a [Mesh Renderer](https://wiki.resonite.com/Component:MeshRenderer "Component:MeshRenderer") to see what it looks like. Don't forget to use a material.

## Examples

[![Three bevel box meshes of different colors and sizes.](https://wiki.resonite.com/images/thumb/4/42/BevelBoxExample.webp/300px-BevelBoxExample.webp.png)](https://wiki.resonite.com/File:BevelBoxExample.webp) A few BevelBoxMesh components with different settings.

The BevelBoxMesh component can be used to create many interesting shapes by mixing different sizes and bevels.

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:BevelBoxMesh&oldid=97870](https://wiki.resonite.com/index.php?title=Component:BevelBoxMesh&oldid=97870)"

Contents