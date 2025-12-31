# ProtoFlux:Atan2

> Source: https://wiki.resonite.com/ProtoFlux:Atan2

Atan2

Y

\*

X

Trigonometry

The **Atan2** node returns the [2-argument arctangent](https://en.wikipedia.org/wiki/Atan2) of the point with the input X and Y coordinates. The output value is the angle between the positive x axis and the point in [the Cartesian coordinate system](https://en.wikipedia.org/wiki/Cartesian_coordinate_system).

![](https://wiki.resonite.com/images/c/c1/SuggestionIcon.svg)

The output value is in [radians](https://en.wikipedia.org/wiki/Radian). If you want a value in degrees, multiply by the [Rad 2 Deg](https://wiki.resonite.com/ProtoFlux:Rad_2_Deg "ProtoFlux:Rad 2 Deg") node.


## Variants

There are many variants of this node. The simplest take 2 scalar numeric-typed values. Some more complicated variants take one scalar and one vector or two same-sized vectors. In each case, the output has the same dimensions as the highest dimension input. Values are calculated element-wise, for example:

If the input Y is 1 and input X is \[2;3\] the output will be \[Atan2(1,2);Atan2(1,3)\].

Similarly if the input Y is \[1;2\] and the input X is \[3;4\] the output will be \[Atan2(1,3);Atan2(2,4)\].

## Inputs

### Y (Pseudo-Generic)

Input Y coordinate value.

### X (Pseudo-Generic)

Input X coordinate value.

## Outputs

### \\* (Pseudo-Generic)

2-argument arctangent of Y and X.

## Further Reading

### Videos

Load video

YouTube

YouTube might collect personal data. [Privacy Policy](https://www.youtube.com/howyoutubeworks/user-settings/privacy/)

ContinueDismiss

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:Atan2&oldid=87842](https://wiki.resonite.com/index.php?title=ProtoFlux:Atan2&oldid=87842)"

Contents