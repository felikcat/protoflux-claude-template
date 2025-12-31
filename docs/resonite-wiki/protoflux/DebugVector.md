# ProtoFlux:DebugVector

> Source: https://wiki.resonite.com/ProtoFlux:DebugVector

Debug Vector

\*

Next

Position

Vector

Color

RadiusRatio

Duration

Debug

Debug Vector is a ProtoFlux node that creates a vector line going from the `Position` into the direction of the `Vector` in global space. The visual will appear under the [Root](https://wiki.resonite.com/Root "Root") of a world. In most cases, the debug visuals will be drawn over most materials, letting you see them easily.

This is useful for Vector debugging.

See also: [Coordinate spaces](https://wiki.resonite.com/Coordinate_spaces "Coordinate spaces")

## Inputs

### \\* ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Create the Vector debug visual with the given parameters.

### Position ( [float3](https://wiki.resonite.com/Type:Float3 "Type:Float3"))

The point of the vector visual in global space.

### Vector ( [float3](https://wiki.resonite.com/Type:Float3 "Type:Float3"))

The direction of the vector visual in global space.

### Color ( [colorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX"))

The color the visual should be.

### RadiusRatio ( [float](https://wiki.resonite.com/Type:Float "Type:Float"))

The distance from the center line to the outside edge in meters. (Also called thickness)

### Duration ( [float](https://wiki.resonite.com/Type:Float "Type:Float"))

How long the visual should appear in seconds.

## Outputs

### Next ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Fires after \* ( [Call](https://wiki.resonite.com/Impulses "Impulses")) has been called and the visual was created.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:DebugVector&oldid=109635](https://wiki.resonite.com/index.php?title=ProtoFlux:DebugVector&oldid=109635)"

Contents