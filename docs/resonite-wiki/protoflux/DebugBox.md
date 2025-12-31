# ProtoFlux:DebugBox

> Source: https://wiki.resonite.com/ProtoFlux:DebugBox

Debug Box

\*

Next

Point

Size

Orientation

Color

Duration

Debug

Debug Box is a ProtoFlux node that when called will make a cube visual at the global coordinates with a size provided and will appear for a duration in seconds. The visual will appear under the [Root](https://wiki.resonite.com/Root "Root") of a world. In most cases, the debug visuals will be drawn over most materials, letting you see them easily.

See also: [Coordinate spaces](https://wiki.resonite.com/Coordinate_spaces "Coordinate spaces")

## Inputs

### \\* ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Call this to spawn a debug box visual in the root of the world with the provided parameters.

### Position ( [float3](https://wiki.resonite.com/Type:Float3 "Type:Float3"))

The position in global space for the debug visual. Default at the node.

### Size ( [float3](https://wiki.resonite.com/Type:Float3 "Type:Float3"))

The size of the box visual in meters.

### Orientation ( [floatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ"))

The Rotation in global space for the debug visual. Default 0.

### ForwardColor ( [colorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX"))

The color for the box visual generated. Defaults to white.

### Duration ( [float](https://wiki.resonite.com/Type:Float "Type:Float"))

How long the debug box visual appears for in seconds.

## Outputs

### Next ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Fires after \* ( [Call](https://wiki.resonite.com/Impulses "Impulses")) is impulsed and the visual was created successfully.

## Examples

- [An example of a visual created by the Debug Box node with the default colors that is rotated in a random orientation.](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=Protoflux_example_Debug_Box.webp "File:Protoflux example Debug Box.webp")

An example of a visual created by the Debug Box node with the default colors that is rotated in a random orientation.


Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:DebugBox&oldid=109625](https://wiki.resonite.com/index.php?title=ProtoFlux:DebugBox&oldid=109625)"

Contents