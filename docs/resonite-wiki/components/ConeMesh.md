# Component:ConeMesh

> Source: https://wiki.resonite.com/Component:ConeMesh

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:ConeMesh&diff=97903) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/4/4f/ConeMeshComponent.png/510px-ConeMeshComponent.png)](https://wiki.resonite.com/File:ConeMeshComponent.png) **Cone Mesh** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ConeMesh** component acts as a source of geometry for rendering a cone with x sides with an optionally flat end.

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
| `Height` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Determines the height of the cone. |
| `RadiusBase` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Determines the width of the cone's base. |
| `RadiusTop` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Determines the width from the top of the cone. |
| `Sides` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | How smooth the roundness of the mesh. |
| `Caps` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to cap the ends with geometry or leave them open. |
| `FlatShading` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Toggles mesh smooth shading. |
| `UVScale` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The scale of the procedural UV map. Larger values make textures appear smaller on the mesh's surface, and vice versa. |

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

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ConeMesh&oldid=97903](https://wiki.resonite.com/index.php?title=Component:ConeMesh&oldid=97903)"

Contents