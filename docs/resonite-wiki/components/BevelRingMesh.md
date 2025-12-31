# Component:BevelRingMesh

> Source: https://wiki.resonite.com/Component:BevelRingMesh

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/a/af/BevelRingMeshComponent.png/510px-BevelRingMeshComponent.png)](https://wiki.resonite.com/File:BevelRingMeshComponent.png) **Bevel Ring Mesh** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

Bevel Ring Mesh is a component that can create an circle or part of a circle in the form of a 3D strip that can have beveled edges. The geometry made by this component can be viewed by inserting the component into a [MeshRenderer](https://wiki.resonite.com/Component:MeshRenderer "Component:MeshRenderer").

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
| `Arc` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How long the strip continues from the starting point defined by `ArcOffset` |
| `ArcOffset` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The degree that the start point of the strip is at. |
| `Radius` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The distance the middle of the strip is from the curvature center. |
| `Width` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How wide the curved strip is |
| `Thickness` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The thickness of the curved strip. |
| `Tilt` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to bend the strip from a flat orientation to inwards/outwards slop from/towards the center. Is in degrees. |
| `Segments` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | how many bends are generated in the curve. Bigger values result in smoother curve in exchange for performance. |

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

Used in old content that used another platform's logo. Which was made of 8 pieces like Resonite's logo. It also is used to make holo Frisbees.

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:BevelRingMesh&oldid=97872](https://wiki.resonite.com/index.php?title=Component:BevelRingMesh&oldid=97872)"

Contents