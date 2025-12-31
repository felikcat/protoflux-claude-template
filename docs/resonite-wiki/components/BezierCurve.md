# Component:BezierCurve

> Source: https://wiki.resonite.com/Component:BezierCurve

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:BezierCurve&diff=91506) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/f/f9/BezierCurveComponent.png/510px-BezierCurveComponent.png)](https://wiki.resonite.com/File:BezierCurveComponent.png) **Bezier Curve** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

Bezier curve is used along with [Bezier Tube Mesh](https://wiki.resonite.com/Component:BezierTubeMesh "Component:BezierTubeMesh") to define the array of curve points that control the mesh's shape. See [Bezier Tube Mesh](https://wiki.resonite.com/Component:BezierTubeMesh "Component:BezierTubeMesh") for a full example.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Points` | _direct_ **[SyncRelayList\`1](https://wiki.resonite.com/index.php?title=Type:SyncRelayList%601&action=edit&redlink=1 "Type:SyncRelayList`1 (page does not exist)") < [CurvePoint](https://wiki.resonite.com/Component:CurvePoint "Component:CurvePoint") >** | A list of controlling Curve Points. |
| `CoordinateSpace` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The [Coordinate Space](https://wiki.resonite.com/Coordinate_spaces "Coordinate spaces") in which to do curve calculations in. |
| `AssignCurveData` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[SyncCurve\`1](https://wiki.resonite.com/index.php?title=Type:SyncCurve%601&action=edit&redlink=1 "Type:SyncCurve`1 (page does not exist)") < [Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3") >** | The list to fill with curve data, which is the `Points` field of a [Bezier Tube Mesh](https://wiki.resonite.com/Component:BezierTubeMesh "Component:BezierTubeMesh"). |

Fields
Collapse

## Usage

## Examples

- [![Example (part 2) of a bezier tube mesh setup](https://wiki.resonite.com/images/thumb/1/11/BezierTubeMesh_Example_2.png/397px-BezierTubeMesh_Example_2.png)](https://wiki.resonite.com/File:BezierTubeMesh_Example_2.png "Example (part 2) of a bezier tube mesh setup")

Example (part 2) of a bezier tube mesh setup


## Related Components

- [Curve Point](https://wiki.resonite.com/Component:CurvePoint "Component:CurvePoint")
- [Bezier Tube Mesh](https://wiki.resonite.com/Component:BezierTubeMesh "Component:BezierTubeMesh")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:BezierCurve&oldid=91506](https://wiki.resonite.com/index.php?title=Component:BezierCurve&oldid=91506)"

Contents