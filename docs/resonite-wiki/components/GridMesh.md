# Component:GridMesh

> Source: https://wiki.resonite.com/Component:GridMesh

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:GridMesh&diff=113644) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/1/19/GridMeshComponent.png/510px-GridMeshComponent.png)](https://wiki.resonite.com/File:GridMeshComponent.png) **Grid Mesh** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **GridMesh** component generates a procedural mesh for use with [Mesh Renderers](https://wiki.resonite.com/Component:MeshRenderer "Component:MeshRenderer") that is like a [Quad Mesh](https://wiki.resonite.com/Component:QuadMesh "Component:QuadMesh") but has multiple squares instead of being one big square.

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
| `Points` | **[Int2](https://wiki.resonite.com/Type:Int2 "Type:Int2")** | how many vertex points should be used on each axis to make the grid of quads |
| `Size` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | how big the grid is scale wise. |
| `FlatShading` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Disable smooth shading |
| `DisplacementMagnitude` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How far to displace the grid texture using `DisplacementTexture` |
| `DisplacementTexture` | **[Texture2D](https://wiki.resonite.com/Type:Texture2D "Type:Texture2D")** | The texture to use for displacement. must be set to Uncompressed. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `BakeMesh:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Bake meshes is a sync method that creates a static mesh component with this component, replaces all references to this component with the static mesh component, then deletes this component. |

Triggers
Collapse

## Usage

Attach to a slot and insert into a [Component:MeshRenderer](https://wiki.resonite.com/Component:MeshRenderer "Component:MeshRenderer") to see the geometry. Don't forget to use a [Material](https://wiki.resonite.com/Material "Material").

## Examples

[![](https://wiki.resonite.com/images/thumb/3/3d/DisplacementMapExample1.png/300px-DisplacementMapExample1.png)](https://wiki.resonite.com/File:DisplacementMapExample1.png) Example of using a texture to set an displacement map.

The DisplacementTexture field can be used to create terrain from a greyscale image.

Notes: Make sure that both Readable and DirectLoad is set to True on the texture.

[![](https://wiki.resonite.com/images/thumb/d/de/DisplacementExample2.png/300px-DisplacementExample2.png)](https://wiki.resonite.com/File:DisplacementExample2.png) Close up of inspectors

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:GridMesh&oldid=113644](https://wiki.resonite.com/index.php?title=Component:GridMesh&oldid=113644)"

Contents