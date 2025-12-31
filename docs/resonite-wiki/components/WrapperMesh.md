# Component:WrapperMesh

> Source: https://wiki.resonite.com/Component:WrapperMesh

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:WrapperMesh&diff=98126) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/d/db/WrapperMesh.webp/510px-WrapperMesh.webp.png)](https://wiki.resonite.com/File:WrapperMesh.webp) **Wrapper Mesh** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The WrapperMesh is a procedural mesh that copies an existing mesh, making it act like a procedural mesh instead through this component.

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
| `Mesh` | **[Mesh](https://wiki.resonite.com/Type:Mesh "Type:Mesh")** | The mesh to wrap |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `BakeMesh:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Bake meshes is a sync method that creates a static mesh component with this component, replaces all references to this component with the static mesh component, then deletes this component. |

Triggers
Collapse

## Usage

Can be used to make a static mesh have the function of a procedural mesh for components/functions that require procedural meshes.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Component:StaticMesh](https://wiki.resonite.com/Component:StaticMesh "Component:StaticMesh")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:WrapperMesh&oldid=98126](https://wiki.resonite.com/index.php?title=Component:WrapperMesh&oldid=98126)"

Contents