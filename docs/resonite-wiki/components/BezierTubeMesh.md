# Component:BezierTubeMesh

> Source: https://wiki.resonite.com/Component:BezierTubeMesh

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:BezierTubeMesh&diff=97874) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/0/06/BezierTubeMeshComponent.png/510px-BezierTubeMeshComponent.png)](https://wiki.resonite.com/File:BezierTubeMeshComponent.png) **Bezier Tube Mesh** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

Bezier tube mesh is a component that allows for making a continuous tube of geometry that is a Bezier curve shape defined by points.

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
| `Radius` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The radius of the tube (from center to outside). |
| `Points` | _direct_ **[SyncCurve\`1](https://wiki.resonite.com/index.php?title=Type:SyncCurve%601&action=edit&redlink=1 "Type:SyncCurve`1 (page does not exist)") < [Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3") >** | Curve tangent point/handle array used for the generation of this mesh. Editing this via [Mods](https://wiki.resonite.com/Mods "Mods") produces undesirable results where the curve has really sharp bends. |
| `SegmentPoints` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | How many sides the tube mesh has around it's mid section. |
| `StepsPerUnitLength` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | How many bends from point to point the tube should have. |

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

- [![Example (part 1) of a bezier tube mesh setup](https://wiki.resonite.com/images/thumb/d/df/BezierTubeMesh_Example_1.png/480px-BezierTubeMesh_Example_1.png)](https://wiki.resonite.com/File:BezierTubeMesh_Example_1.png "Example (part 1) of a bezier tube mesh setup")

Example (part 1) of a bezier tube mesh setup

- [![Example (part 2) of a bezier tube mesh setup](https://wiki.resonite.com/images/thumb/1/11/BezierTubeMesh_Example_2.png/397px-BezierTubeMesh_Example_2.png)](https://wiki.resonite.com/File:BezierTubeMesh_Example_2.png "Example (part 2) of a bezier tube mesh setup")

Example (part 2) of a bezier tube mesh setup

- [![Example (part 3) of a bezier tube mesh setup](https://wiki.resonite.com/images/thumb/a/ad/BezierTubeMesh_Example_3.png/480px-BezierTubeMesh_Example_3.png)](https://wiki.resonite.com/File:BezierTubeMesh_Example_3.png "Example (part 3) of a bezier tube mesh setup")

Example (part 3) of a bezier tube mesh setup


## Related Components

- [Curve Point](https://wiki.resonite.com/Component:CurvePoint "Component:CurvePoint")
- [Bezier Curve](https://wiki.resonite.com/Component:BezierCurve "Component:BezierCurve")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:BezierTubeMesh&oldid=97874](https://wiki.resonite.com/index.php?title=Component:BezierTubeMesh&oldid=97874)"

Contents