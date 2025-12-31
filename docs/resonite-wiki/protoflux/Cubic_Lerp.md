# ProtoFlux:Cubic Lerp

> Source: https://wiki.resonite.com/ProtoFlux:Cubic_Lerp

(Redirected from [ProtoFlux:Cubic Lerp](https://wiki.resonite.com/index.php?title=ProtoFlux:Cubic_Lerp&redirect=no "ProtoFlux:Cubic Lerp"))

Cubic Lerp

From

\*

To

Lerp

Interpolation

The **Cubic Lerp** takes in 2 tangent points ( [TangentPointFloat](https://wiki.resonite.com/index.php?title=Type:TangentPointFloat&action=edit&redlink=1 "Type:TangentPointFloat (page does not exist)") or [TangentPointDouble](https://wiki.resonite.com/index.php?title=Type:TangentPointDouble&action=edit&redlink=1 "Type:TangentPointDouble (page does not exist)")), and a lerp value to travel from start to finish. This returns the value of a specific point using that lerp value.

![](https://wiki.resonite.com/images/d/dd/InformationIcon.svg)

The types needed are found using the [Pack Tangent Point](https://wiki.resonite.com/ProtoFlux:Pack_To_Tangent_Point "ProtoFlux:Pack To Tangent Point") nodes.


This differs from the [Bezier Curve](https://wiki.resonite.com/ProtoFlux:Bezier_Curve "ProtoFlux:Bezier Curve") node as it attempts to solve a problem with curves, utilizing [Cubic Spline Interpolation](https://en.wikiversity.org/wiki/Cubic_Spline_Interpolation).

## Inputs

### From (Pseudo-Generic)

The start point of this lerp.

### To (Pseudo-Generic)

The end point of this lerp.

### Lerp ( [float](https://wiki.resonite.com/Type:Float "Type:Float"))

The travel point from start to finish.

## Outputs

### \\* (Pseudo-Generic)

Returns the value of a specific point along this lerp value.

## See Also

- Wikipedia's definition of a [spline interpolation](https://en.wikipedia.org/wiki/Spline_interpolation) & [runge's phenomenon](https://en.wikipedia.org/wiki/Runge%27s_phenomenon).
- Wikiversity's [Cubic Spline Interpolation](https://en.wikiversity.org/wiki/Cubic_Spline_Interpolation) page.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:CubicLerp&oldid=109595](https://wiki.resonite.com/index.php?title=ProtoFlux:CubicLerp&oldid=109595)"

Contents