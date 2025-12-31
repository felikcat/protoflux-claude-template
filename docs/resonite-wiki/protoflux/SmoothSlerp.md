# ProtoFlux:SmoothSlerp

> Source: https://wiki.resonite.com/ProtoFlux:SmoothSlerp

Smooth Slerp

Input

\*

Speed

Interpolation

The **Smooth Slerp** node takes in an input value and the speed of which it slerps smoothly towards (starts fast and slows down over time), then returns the value over time.

The "S" part of the slerp stands for "spherical", which means that it deals more with rotations and the values relating to that type of movement ( [floatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ") for reference).

![](https://wiki.resonite.com/images/c/c1/SuggestionIcon.svg)

If you need the slerp to be linear, use the [Constant Slerp](https://wiki.resonite.com/ProtoFlux:Constant_Slerp "ProtoFlux:Constant Slerp") node instead.


## Inputs

### Input (Pseudo-Generic)

The value we want to slerp towards.

### Speed ( [float](https://wiki.resonite.com/Type:Float "Type:Float"))

How fast the slerp should be.

## Outputs

### \\* (Pseudo-Generic)

Returns the value currently being slerped.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:SmoothSlerp&oldid=110755](https://wiki.resonite.com/index.php?title=ProtoFlux:SmoothSlerp&oldid=110755)"

Contents