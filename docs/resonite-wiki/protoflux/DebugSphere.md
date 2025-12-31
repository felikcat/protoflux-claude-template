# ProtoFlux:DebugSphere

> Source: https://wiki.resonite.com/ProtoFlux:DebugSphere

Debug Sphere

\*

Next

Point

Radius

Color

Duration

Debug

Debug Sphere is a ProtoFlux node that when called will make a sphere visual at the global Point ( [float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")) with a radius provided and will appear for a duration in seconds. The visual will appear under the [Root](https://wiki.resonite.com/Root "Root") of a world. In most cases, the debug visuals will be drawn over most materials, letting you see them easily.

See also: [Coordinate spaces](https://wiki.resonite.com/Coordinate_spaces "Coordinate spaces")

### \\* ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Create the Sphere debug visual with the given parameters.

### Point ( [float3](https://wiki.resonite.com/Type:Float3 "Type:Float3"))

The position in global [coordinates](https://wiki.resonite.com/Coordinate_spaces "Coordinate spaces") to put the visual.

### Radius ( [float](https://wiki.resonite.com/Type:Float "Type:Float"))

The radius in meters the visual should be.

### Color ( [colorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX"))

The color the visual should be.

### Duration ( [float](https://wiki.resonite.com/Type:Float "Type:Float"))

How long the visual should appear for.

## Outputs

### Next ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Fires after \* ( [Call](https://wiki.resonite.com/Impulses "Impulses")) is impulsed and the visual was created successfully.

## Examples

- [An example of a visual created by the Debug Sphere node with the default colors.](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=Protoflux_example_Debug_Sphere.webp "File:Protoflux example Debug Sphere.webp")

An example of a visual created by the Debug Sphere node with the default colors.


Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:DebugSphere&oldid=109629](https://wiki.resonite.com/index.php?title=ProtoFlux:DebugSphere&oldid=109629)"

Contents