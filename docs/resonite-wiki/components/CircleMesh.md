# Component:CircleMesh

> Source: https://wiki.resonite.com/Component:CircleMesh

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:CircleMesh&diff=97891) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/2/2c/CircleMeshComponent.png/510px-CircleMeshComponent.png)](https://wiki.resonite.com/File:CircleMeshComponent.png) **Circle Mesh** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

_This article or section is a stub. You can help the Resonite wiki by expanding it._

The **CircleMesh** component procedurally generates a circle mesh for use with a [MeshRenderer](https://wiki.resonite.com/Component:MeshRenderer "Component:MeshRenderer").

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
| `Rotation` | **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | How much to rotate the circle mesh from it's rest position before rendering |
| `Segments` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | How many sides the circle has. |
| `Radius` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How big the circle's radius is. |
| `Arc` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much out of 360 degrees the circle should take up of a full circle. |
| `UVScale` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The scale of the texture detail of the material rendered on this mesh. |
| `ScaleUVWithSize` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to make the detail of the material independent of the size of circle in global space. |
| `TriangleFan` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to make the circle a bunch of triangles that meet in the middle or not. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `BakeMesh:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Bake meshes is a sync method that creates a static mesh component with this component, replaces all references to this component with the static mesh component, then deletes this component. |

Triggers
Collapse

## Usage

Attach this component to a slot, and then put it inside of a [Mesh Renderer component](https://wiki.resonite.com/Component:MeshRenderer "Component:MeshRenderer") to view what it looks like. Don't forget to add a [material](https://wiki.resonite.com/Material "Material") to the mesh renderer.

## Examples

Can be used to make a round platform, or to make a mini disc world.

## Related Components

[Procedural Meshes](https://wiki.resonite.com/Category:Components:Assets:Procedural_Meshes "Category:Components:Assets:Procedural Meshes")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:CircleMesh&oldid=97891](https://wiki.resonite.com/index.php?title=Component:CircleMesh&oldid=97891)"

Contents