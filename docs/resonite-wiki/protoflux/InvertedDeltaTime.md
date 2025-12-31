# ProtoFlux:InvertedDeltaTime

> Source: https://wiki.resonite.com/ProtoFlux:InvertedDeltaTime

1/dT

\*

Time

The `Inverted Delta Time` node returns the frames per second, shown when pulling a display node from it and comparing it to the [Dash's](https://wiki.resonite.com/Dash "Dash") FPS counter.

This is done by taking the reciprocal of delta time: FPS = 1 / dT

![](https://wiki.resonite.com/images/d/dd/InformationIcon.svg)

Not to be confused with [Delta Time](https://wiki.resonite.com/ProtoFlux:Delta_Time "ProtoFlux:Delta Time"), as that node focuses on how long each frame takes before the next one is rendered.


### Example Calculation

For instance, if the delta time (dt) is 0.016 seconds (which is approximately the time per frame for a game running at 60 FPS), the FPS can be calculated as:

FPS = 1/0.016 ≈ 62.5

## Outputs

### \\* ( [float](https://wiki.resonite.com/Type:Float "Type:Float"))

Returns the inverted delta time (1 / dT), showing the amount of frames in a second.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:InvertedDeltaTime&oldid=110075](https://wiki.resonite.com/index.php?title=ProtoFlux:InvertedDeltaTime&oldid=110075)"

Contents