# Component:CurvePoint

> Source: https://wiki.resonite.com/Component:CurvePoint

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/a/a9/CurvePointComponent.png/510px-CurvePointComponent.png)](https://wiki.resonite.com/File:CurvePointComponent.png) **Curve Point** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Curve point is used by being put into a [Bezier Curve](https://wiki.resonite.com/Component:BezierCurve "Component:BezierCurve") component to define the shape of a [Bezier Tube Mesh](https://wiki.resonite.com/Component:BezierTubeMesh "Component:BezierTubeMesh"). See [Bezier Tube Mesh](https://wiki.resonite.com/Component:BezierTubeMesh "Component:BezierTubeMesh") for a full example.

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `LeftTangentSource` | _direct_ **[TransformRelayRef](https://wiki.resonite.com/index.php?title=Type:TransformRelayRef&action=edit&redlink=1 "Type:TransformRelayRef (page does not exist)")** | The left handle of the bezier curve point |
| `RightTangentSource` | _direct_ **[TransformRelayRef](https://wiki.resonite.com/index.php?title=Type:TransformRelayRef&action=edit&redlink=1 "Type:TransformRelayRef (page does not exist)")** | The right handle of the bezier curve point |

Fields
Collapse

## Behavior

## Examples

- [![Example (part 3) of a bezier tube mesh setup](https://wiki.resonite.com/images/thumb/a/ad/BezierTubeMesh_Example_3.png/480px-BezierTubeMesh_Example_3.png)](https://wiki.resonite.com/File:BezierTubeMesh_Example_3.png "Example (part 3) of a bezier tube mesh setup")

Example (part 3) of a bezier tube mesh setup


## See Also

- [Bezier Tube Mesh](https://wiki.resonite.com/Component:BezierTubeMesh "Component:BezierTubeMesh")
- [Bezier Curve](https://wiki.resonite.com/Component:BezierCurve "Component:BezierCurve")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:CurvePoint&oldid=91505](https://wiki.resonite.com/index.php?title=Component:CurvePoint&oldid=91505)"

Contents