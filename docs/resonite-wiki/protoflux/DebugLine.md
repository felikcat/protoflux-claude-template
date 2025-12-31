# ProtoFlux:DebugLine

> Source: https://wiki.resonite.com/ProtoFlux:DebugLine

Debug Line

\*

Next

Point0

Point1

Color

Radius

Duration

Debug

Debug Line is a ProtoFlux node that creates a line going between Point0 to Point1 in global space. The visual will appear under the [Root](https://wiki.resonite.com/Root "Root") of a world. In most cases, the debug visuals will be drawn over most materials, letting you see them easily.

This is useful for Vector debugging.

See also: [Coordinate spaces](https://wiki.resonite.com/Coordinate_spaces "Coordinate spaces")

## Inputs

### \\* ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Create the Line debug visual with the given parameters.

### Point0 ( [float3](https://wiki.resonite.com/Type:Float3 "Type:Float3"))

The first point of the line visual in global space.

### Point1 ( [float3](https://wiki.resonite.com/Type:Float3 "Type:Float3"))

The second point of the line visual in global space.

### Color ( [colorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX"))

The color the visual should be.

### Radius ( [float](https://wiki.resonite.com/Type:Float "Type:Float"))

The distance from the center line to the outside edge in meters.

### Duration ( [float](https://wiki.resonite.com/Type:Float "Type:Float"))

How long the visual should appear in seconds.

## Outputs

### Next ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Fires after \* ( [Call](https://wiki.resonite.com/Impulses "Impulses")) has been called and the visual was created.

## Examples

- [An example of a visual created by the Debug Line node with the default colors that is rotated in a random orientation.](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=Protoflux_example_Debug_Line.webp "File:Protoflux example Debug Line.webp")

An example of a visual created by the Debug Line node with the default colors that is rotated in a random orientation.


Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:DebugLine&oldid=109627](https://wiki.resonite.com/index.php?title=ProtoFlux:DebugLine&oldid=109627)"

Contents