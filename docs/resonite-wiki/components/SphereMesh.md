# Component:SphereMesh

> Source: https://wiki.resonite.com/Component:SphereMesh

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:SphereMesh&diff=98424) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/2/22/SphereMeshComponent.png/510px-SphereMeshComponent.png)](https://wiki.resonite.com/File:SphereMeshComponent.png) **Sphere Mesh** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **SphereMesh** component generates a sphere mesh for use with a [MeshRenderer](https://wiki.resonite.com/MeshRenderer_(Component) "MeshRenderer (Component)").

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
| `Radius` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The radius of the sphere mesh. |
| `Segments` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | how many vertical lined edges the sphere has |
| `Rings` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | how many horizontal lined edges the sphere has. |
| `Shading` | **[Shading](https://wiki.resonite.com/Type:Shading "Type:Shading")** | Whether to have smooth or flat shading |
| `UVScale` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | the scale of material detail on the surface |
| `DualSided` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | whether to make a second set of polygons that shows the mesh when viewed from the inside. |

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

Can be used to render anything round like balls, planets, or suns.

## See Also

[Sphere Collider](https://wiki.resonite.com/Component:SphereCollider "Component:SphereCollider")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:SphereMesh&oldid=98424](https://wiki.resonite.com/index.php?title=Component:SphereMesh&oldid=98424)"

Contents