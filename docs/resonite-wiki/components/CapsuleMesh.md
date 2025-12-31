# Component:CapsuleMesh

> Source: https://wiki.resonite.com/Component:CapsuleMesh

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:CapsuleMesh&diff=97889) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/8/88/CapsuleMeshComponent.png/510px-CapsuleMeshComponent.png)](https://wiki.resonite.com/File:CapsuleMeshComponent.png) **Capsule Mesh** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

Creates a mesh that is a cylinder with rounded ends instead of flat ends.

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
| `Radius` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Determines the roundness of the mesh. |
| `Height` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Determines how tall the mesh is. |
| `Segments` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Determines the smoothness. |
| `Rings` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Determines the smoothness of the top & bottom of the mesh. |
| `Shading` | **[Shading](https://wiki.resonite.com/Type:Shading "Type:Shading")** | Changes the mesh shading. |
| `UVScale` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The inverse of the size the material should appear on the surface as. |
| `DualSided` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Makes the mesh dual sided. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `BakeMesh:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Bake meshes is a sync method that creates a static mesh component with this component, replaces all references to this component with the static mesh component, then deletes this component. |

Triggers
Collapse

## Usage

Add this mesh to a mesh renderer component along with a material to view it

## Examples

A collider with the same shape as this mesh is used for the physics locomotion of the user.

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:CapsuleMesh&oldid=97889](https://wiki.resonite.com/index.php?title=Component:CapsuleMesh&oldid=97889)"

Contents