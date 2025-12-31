# ProtoFlux:PointOnCircle

> Source: https://wiki.resonite.com/ProtoFlux:PointOnCircle

Point On Circle

NormalizedPosition

\*

Radius

Geometry 2D

The **Point On Circle** node returns the point a fractional part of the trace along a circle path of a given radius.

## Inputs

### NormalizedPosition ( [float](https://wiki.resonite.com/Type:Float "Type:Float"))

Position of the point along the path. Essentially represents an angle of `2*pi*NormalizedPosition` radians.

### Radius ( [float](https://wiki.resonite.com/Type:Float "Type:Float"))

Radius of the circle to trace along.

## Outputs

### \\* ( [float2](https://wiki.resonite.com/Type:Float2 "Type:Float2"))

The point that is `NormalizedPosition` along the path of the circle, starting at the top point and tracing clockwise. The exact point returned is `(sin(2 * pi * NormalizedPosition), cos(2 * pi * NormalizedPosition))`.

## Examples

- [![Examples of the Point On Circle node. The small discrepencies on quarter and full turns are due to floating point inaccuracies.](https://wiki.resonite.com/images/thumb/8/8e/Protoflux_Example_Point_On_Circle.webp/297px-Protoflux_Example_Point_On_Circle.webp.png)](https://wiki.resonite.com/File:Protoflux_Example_Point_On_Circle.webp "Examples of the Point On Circle node. The small discrepencies on quarter and full turns are due to floating point inaccuracies.")

Examples of the Point On Circle node. The small discrepencies on quarter and full turns are due to floating point inaccuracies.


Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:PointOnCircle&oldid=110461](https://wiki.resonite.com/index.php?title=ProtoFlux:PointOnCircle&oldid=110461)"

Contents