# ProtoFlux:InvertedSmoothDeltaTime

> Source: https://wiki.resonite.com/ProtoFlux:InvertedSmoothDeltaTime

Smooth 1/dT

\*

Time

The `Inverted Smooth Delta Time` node returns the frames per second, shown when pulling a display node from it and comparing it to the [Dash's](https://wiki.resonite.com/Dash "Dash") FPS counter. This will attempt to adjust to any lag or stutters by smoothing out the differences between the results.

This is done by taking the reciprocal of delta time: FPS = 1 / dT (+ some smoothing algorithm)

![](https://wiki.resonite.com/images/d/dd/InformationIcon.svg)

Not to be confused with [Smooth Delta Time](https://wiki.resonite.com/ProtoFlux:Smooth_Delta_Time "ProtoFlux:Smooth Delta Time"), as that node focuses on how long each frame takes before the next one is rendered and adjusts smoothly between the difference.


### Example Calculation

For instance, if the delta time (dt) is 0.016 seconds (which is approximately the time per frame for a game running at 60 FPS), the FPS can be calculated as:

FPS = 1/0.016 ≈ 62.5

## Outputs

### \\* ( [float](https://wiki.resonite.com/Type:Float "Type:Float"))

Returns the inverted and smoothed delta time (1 / dT), showing the amount of frames in a second.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:InvertedSmoothDeltaTime&oldid=110083](https://wiki.resonite.com/index.php?title=ProtoFlux:InvertedSmoothDeltaTime&oldid=110083)"

Contents