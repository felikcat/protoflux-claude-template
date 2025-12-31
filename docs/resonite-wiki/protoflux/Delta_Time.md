# ProtoFlux:Delta Time

> Source: https://wiki.resonite.com/ProtoFlux:Delta_Time

(Redirected from [ProtoFlux:Delta Time](https://wiki.resonite.com/index.php?title=ProtoFlux:Delta_Time&redirect=no "ProtoFlux:Delta Time"))

dT

\*

Time

The `Delta Time` node returns the change of time between two world updates, specifically the time between the current update and the one before.

![](https://wiki.resonite.com/images/c/c1/SuggestionIcon.svg)

There is an alternative node called [Smooth Delta Time](https://wiki.resonite.com/ProtoFlux:Smooth_Delta_Time "ProtoFlux:Smooth Delta Time") that tries to smooth out this result when getting lag or frame stutters.


This [Unity Documentation about Delta Time](https://docs.unity3d.com/ScriptReference/Time-deltaTime.html) may be relevant in helping understand what this does. And following that, this has an excellent explanation about [Time Frame Management](https://docs.unity3d.com/Manual/TimeFrameManagement.html), which in general may help with working with this node in your content.

### Uses

Using this node, you can make an accumulator or a timer using the frames here and storing them to a variable and adding them every frame.

## Outputs

### \\* ( [float](https://wiki.resonite.com/Type:Float "Type:Float"))

The difference in time between this frame and the last frame.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:DeltaTime&oldid=109663](https://wiki.resonite.com/index.php?title=ProtoFlux:DeltaTime&oldid=109663)"

Contents