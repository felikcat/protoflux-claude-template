# ProtoFlux:SmoothDeltaTime

> Source: https://wiki.resonite.com/ProtoFlux:SmoothDeltaTime

Smooth dT

\*

Time

The `Smooth Delta Time` node returns the change of time between two world updates, specifically the time between the current update and the one before. This node also does another step and tries to account for lag or stutters, smoothly changing the amount of time to match that change.

![](https://wiki.resonite.com/images/c/c1/SuggestionIcon.svg)

There is an alternative node called [Delta Time](https://wiki.resonite.com/ProtoFlux:Delta_Time "ProtoFlux:Delta Time") that just returns the result.


This [Unity Documentation about Smooth Delta Time](https://docs.unity3d.com/ScriptReference/Time-smoothDeltaTime.html) may be relevant in helping understand what this does. And following that, this has an excellent explanation about [Time Frame Management](https://docs.unity3d.com/Manual/TimeFrameManagement.html), which in general may help with working with this node in your content.

### Uses

Using this node, you can make an accumulator or a timer using the frames here and storing them to a variable and adding them every frame.

## Outputs

### \\* ( [float](https://wiki.resonite.com/Type:Float "Type:Float"))

The smoothed difference in time between this frame and the last frame.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:SmoothDeltaTime&oldid=110753](https://wiki.resonite.com/index.php?title=ProtoFlux:SmoothDeltaTime&oldid=110753)"

Contents