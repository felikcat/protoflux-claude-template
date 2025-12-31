# Component:IcoSphereMesh

> Source: https://wiki.resonite.com/Component:IcoSphereMesh

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:IcoSphereMesh&diff=97953) which are not marked for translation.

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

The vertex count on a generated **IcoSphereMesh** is 20×4n, where n is `Subdivisions` — this may result in extremely large vertex counts for seemingly small values of `Subdivisions` — **Please use caution!**

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/a/ad/IcoSphereMeshComponent.png/510px-IcoSphereMeshComponent.png)](https://wiki.resonite.com/File:IcoSphereMeshComponent.png) **IcoSphereMesh** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **IcoSphereMesh** component procedurally generates a icosahedron mesh for use with a MeshRenderer, according to the parameters provided.

As of [Version 2020.10.25.1103](https://github.com/Frooxius/NeosPublic/issues/1206), this value is clamped in the range \[0,8\] to prevent accidentally creating a mesh with an excessive number of vertices.

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
| `Radius` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Radius of the IcoSphere |
| `Subdivisions` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Number of IcoSphere subdivisions — Values are clamped in the range \[0,8\] |
| `FlatShading` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Use flat/faceted shading instead of smooth shading. |
| `FlatFaceExtrude` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Distance to extrude faces after being generated. Creates an "Exploded" appearance |
| `FlatFaceScale` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Scale of individual faces, relative to their base size. |

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

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Component:SphereMesh](https://wiki.resonite.com/Component:SphereMesh "Component:SphereMesh")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:IcoSphereMesh&oldid=97953](https://wiki.resonite.com/index.php?title=Component:IcoSphereMesh&oldid=97953)"

Contents