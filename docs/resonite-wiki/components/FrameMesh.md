# Component:FrameMesh

> Source: https://wiki.resonite.com/Component:FrameMesh

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:FrameMesh&diff=97935) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/0/01/FrameMeshComponent.png/510px-FrameMeshComponent.png)](https://wiki.resonite.com/File:FrameMeshComponent.png) **Frame Mesh** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **FrameMesh** component generates a procedural mesh that is like a flat polygon 2d frame for use with [Mesh Renderers](https://wiki.resonite.com/Component:MeshRenderer "Component:MeshRenderer").

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
| `ContentSize` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The size of interior object. usually driven by [Asset Frames](https://wiki.resonite.com/Component:AssetFrameSlot "Component:AssetFrameSlot") |
| `Thickness` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How thick the frame should be, expanding outwards from the center content. |
| `UVScale` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | How big the procedural UV map should be, which influences material detail and color map scales. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `BakeMesh:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Bake meshes is a sync method that creates a static mesh component with this component, replaces all references to this component with the static mesh component, then deletes this component. |

Triggers
Collapse

## Usage

Attach to a slot, and give it `ContentSize` and `Thickness`. Then put into a [Mesh Renderer](https://wiki.resonite.com/Component:MeshRenderer "Component:MeshRenderer") with a [material](https://wiki.resonite.com/Material "Material") to view it.

## Examples

Used in [asset frames](https://wiki.resonite.com/Component:AssetFrameSlot "Component:AssetFrameSlot") like picture frames and audio placement frames.

## Related Components

- [AssetFrameSlot](https://wiki.resonite.com/Component:AssetFrameSlot "Component:AssetFrameSlot")
- [IAsset Type](https://wiki.resonite.com/Type:IAsset%601 "Type:IAsset`1")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:FrameMesh&oldid=97935](https://wiki.resonite.com/index.php?title=Component:FrameMesh&oldid=97935)"

Contents