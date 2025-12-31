# ProtoFlux:DebugTriangle

> Source: https://wiki.resonite.com/ProtoFlux:DebugTriangle

Debug Triangle

\*

Next

Point0

Point1

Point2

Color

Duration

Debug

Debug Triangle is a ProtoFlux node that when called will make a triangle visual using 3 global Points `Point0`, `Point1`, and `Point2`, being ( [float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")) and will appear for a duration in seconds. The visual will appear under the [Root](https://wiki.resonite.com/Root "Root") of a world. In most cases, the debug visuals will be drawn over most materials, letting you see them easily.

See also: [Coordinate spaces](https://wiki.resonite.com/Coordinate_spaces "Coordinate spaces")

### \\* ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Create the Triangle debug visual with the given parameters.

### Point0 ( [float3](https://wiki.resonite.com/Type:Float3 "Type:Float3"))

The position in global [coordinates](https://wiki.resonite.com/Coordinate_spaces "Coordinate spaces") to put the first point of the visual triangle.

### Point1 ( [float3](https://wiki.resonite.com/Type:Float3 "Type:Float3"))

The position in global [coordinates](https://wiki.resonite.com/Coordinate_spaces "Coordinate spaces") to put the second point of the visual triangle.

### Point2( [float3](https://wiki.resonite.com/Type:Float3 "Type:Float3"))

The position in global [coordinates](https://wiki.resonite.com/Coordinate_spaces "Coordinate spaces") to put the third point of the visual triangle.

### Color ( [colorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX"))

The color the visual should be.

### Duration ( [float](https://wiki.resonite.com/Type:Float "Type:Float"))

How long the visual should appear for.

## Outputs

### Next ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Fires after \* ( [Call](https://wiki.resonite.com/Impulses "Impulses")) is impulsed and the visual was created successfully.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:DebugTriangle&oldid=109633](https://wiki.resonite.com/index.php?title=ProtoFlux:DebugTriangle&oldid=109633)"

Contents