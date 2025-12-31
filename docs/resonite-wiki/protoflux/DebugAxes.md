# ProtoFlux:DebugAxes

> Source: https://wiki.resonite.com/ProtoFlux:DebugAxes

Debug Axes

\*

Next

Position

Rotation

Length

RightColor

UpColor

ForwardColor

Duration

Debug

Debug Axes is a ProtoFlux node that when called will make a 3 arrows visual similar to a [Gizmo](https://wiki.resonite.com/Gizmo "Gizmo") at the global coordinates with the arrows having the length provided and will appear for a duration in seconds. The visual will appear under the [Root](https://wiki.resonite.com/Root "Root") of a world. In most cases, the debug visuals will be drawn over most materials, letting you see them easily.

See also: [Coordinate spaces](https://wiki.resonite.com/Coordinate_spaces "Coordinate spaces")

## Inputs

### \\* ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Call this to spawn a debug axes visual in the root of the world with the provided parameters.

### Position ( [float3](https://wiki.resonite.com/Type:Float3 "Type:Float3"))

The position in global space for the debug visual. Default at the node.

### Rotation ( [floatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ"))

The Rotation in global space for the debug visual. Default at the node.

### Length ( [float](https://wiki.resonite.com/Type:Float "Type:Float"))

The length of the arrows for the debug visual in meters.

### RightColor ( [colorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX"))

The color for the debug axes in the (1,0,0) direction. Also known as the red arrow on a [Gizmo](https://wiki.resonite.com/Gizmo "Gizmo"). Defaults to red.

### UpColor ( [colorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX"))

The color for the debug axes in the (0,1,0) direction. Also known as the green arrow on a [Gizmo](https://wiki.resonite.com/Gizmo "Gizmo"). Defaults to green.

### ForwardColor ( [colorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX"))

The color for the debug axes in the (0,0,1) direction. Also known as the blue arrow on a [Gizmo](https://wiki.resonite.com/Gizmo "Gizmo"). Defaults to blue.

### Duration ( [float](https://wiki.resonite.com/Type:Float "Type:Float"))

How long the debug axes visual appears for in seconds.

## Outputs

### Next ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Fires after \* ( [Call](https://wiki.resonite.com/Impulses "Impulses")) is impulsed and the gizmo was created successfully.

## Examples

- [An example of a visual created by the Debug Axes node with the default colors that is rotated in a random orientation.](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=Protoflux_example_Debug_Axes.webp "File:Protoflux example Debug Axes.webp")

An example of a visual created by the Debug Axes node with the default colors that is rotated in a random orientation.


Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:DebugAxes&oldid=109623](https://wiki.resonite.com/index.php?title=ProtoFlux:DebugAxes&oldid=109623)"

Contents