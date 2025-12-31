# ProtoFlux:Angle

> Source: https://wiki.resonite.com/ProtoFlux:Angle

°

(angle)

A

\*

B

Vectors

The **Angle** node takes in 2 vectors (rays or directions) and returns the difference between the 2 provided vectors using angles in degrees as a [float](https://wiki.resonite.com/Type:Float "Type:Float").

The vectors you provide are normalized (but not clamped), which means each value will be between `-1` and `1`, with resulting degrees of `0` (if the 2 vectors are so close to each other that there is effectively no separation, thus no angle) all the way to `180` (if the 2 vectors are so far apart that they are a straight line) respectively.

![](https://wiki.resonite.com/images/c/c1/SuggestionIcon.svg)

If you're using 2D vectors and need to know the sign of the angle (i.e. whether the second vector is closer clockwise or counterclockwise to the first), use [DeltaAngle](https://wiki.resonite.com/ProtoFlux:DeltaAngle "ProtoFlux:DeltaAngle").


## Inputs

### A (Pseudo-Generic)

The first provided vector.

### B (Pseudo-Generic)

The second provided vector.

## Outputs

### \\* ( [float](https://wiki.resonite.com/Type:Float "Type:Float"))

Returns the difference between the 2 provided vectors using angles in degrees.

## See Also

- Wikipedia's definition of an [angle](https://en.wikipedia.org/wiki/Angle).

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:Angle&oldid=113280](https://wiki.resonite.com/index.php?title=ProtoFlux:Angle&oldid=113280)"

Contents