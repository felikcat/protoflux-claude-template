# Component:BevelStripeMesh

> Source: https://wiki.resonite.com/Component:BevelStripeMesh

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/e/e3/BevelStripeMeshComponent.png/510px-BevelStripeMeshComponent.png)](https://wiki.resonite.com/File:BevelStripeMeshComponent.png) **Bevel Stripe Mesh** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Bevel Stripe Mesh is a component that generates Mesh data for cube with a different bevel depth on the top left edge and bottom right edge of the cube. It can also be indented in the middle on two opposite sides.

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
| `Width` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The width of the cube |
| `Height` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | the height of the cube |
| `Thickness` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | the length of the cube. |
| `SlantLeft` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | the Bevel angle of the length wise edge on the top left. |
| `SlantRight` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | the Bevel angle of the length wise edge on the bottom right. |
| `Relief` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to indent the cube in the center. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `BakeMesh:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Bake meshes is a sync method that creates a static mesh component with this component, replaces all references to this component with the static mesh component, then deletes this component. |

Triggers
Collapse

## Usage

The geometry this generates can be viewed by inserting the component into a [Mesh Renderer component](https://wiki.resonite.com/Component:MeshRenderer "Component:MeshRenderer"). Don't forget to use a material with the mesh renderer.

## Examples

Used for the visuals of the ToolShelves that are used on most avatars.

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:BevelStripeMesh&oldid=97873](https://wiki.resonite.com/index.php?title=Component:BevelStripeMesh&oldid=97873)"

Contents