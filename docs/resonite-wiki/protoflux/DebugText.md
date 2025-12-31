# ProtoFlux:DebugText

> Source: https://wiki.resonite.com/ProtoFlux:DebugText

Debug Text

\*

Next

Point

Text

Size

Color

Duration

Debug

Debug Text is a ProtoFlux node that when called will make a text visual at a global Point ( [float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")) and will appear for a duration in seconds. The text that appears will always face in the direction toward you the moment this node is called. The visual will appear under the [Root](https://wiki.resonite.com/Root "Root") of a world. In most cases, the debug visuals will be drawn over most materials, letting you see them easily.

See also: [Coordinate spaces](https://wiki.resonite.com/Coordinate_spaces "Coordinate spaces")

### \\* ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Create the Text debug visual with the given parameters.

### Point ( [float3](https://wiki.resonite.com/Type:Float3 "Type:Float3"))

The position in global [coordinates](https://wiki.resonite.com/Coordinate_spaces "Coordinate spaces") to put the visual.

### Text ( [string](https://wiki.resonite.com/Type:String "Type:String"))

The text to display on the visual.

### Size ( [float](https://wiki.resonite.com/Type:Float "Type:Float"))

The size the visual should be.

### Color ( [colorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX"))

The color the visual should be.

### Duration ( [float](https://wiki.resonite.com/Type:Float "Type:Float"))

How long the visual should appear for.

## Outputs

### Next ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Fires after \* ( [Call](https://wiki.resonite.com/Impulses "Impulses")) is impulsed and the visual was created successfully.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:DebugText&oldid=109631](https://wiki.resonite.com/index.php?title=ProtoFlux:DebugText&oldid=109631)"

Contents