# Component:QuadMesh

> Source: https://wiki.resonite.com/Component:QuadMesh

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:QuadMesh&diff=98028) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/0/0a/QuadMeshComponent.png/510px-QuadMeshComponent.png)](https://wiki.resonite.com/File:QuadMeshComponent.png) **Quad Mesh** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

Quad mesh is a component that generates mesh data procedurally that makes a flat 2D square.

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
| `Rotation` | **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | How to rotate the quad in local space. |
| `Size` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The size of the quad in local space. |
| `UVOffset` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The added offset to the UVs. |
| `UVScale` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The scale of the UVs from the bottom left. |
| `ScaleUVWithSize` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to scale uv mapping with `Size` |
| `DualSided` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to make a second pair of triangles that are visible from the opposite side. |
| `UseVertexColors` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to use vertex colors which can be read by materials. |
| `UpperLeftColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | Upper left vertex color. |
| `LowerLeftColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | Lower left vertex color. |
| `LowerRightColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | Lower right vertex color. |
| `UpperRightColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | Upper right vertex color. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `BakeMesh:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Bake meshes is a sync method that creates a static mesh component with this component, replaces all references to this component with the static mesh component, then deletes this component. |

Triggers
Collapse

## Usage

Attach to a [slot](https://wiki.resonite.com/Slot "Slot") and insert into a [Mesh Renderer](https://wiki.resonite.com/Component:MeshRenderer "Component:MeshRenderer") with a [material](https://wiki.resonite.com/Materials "Materials") to view it.

## Examples

Floors, walls, paper leaflets, screens, anything flat and thin.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:QuadMesh&oldid=98028](https://wiki.resonite.com/index.php?title=Component:QuadMesh&oldid=98028)"

Contents