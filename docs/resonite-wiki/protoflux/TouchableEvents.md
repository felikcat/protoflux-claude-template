# ProtoFlux:TouchableEvents

> Source: https://wiki.resonite.com/ProtoFlux:TouchableEvents

Touchable Events

Pressed

Hover

Touch

Point

Tip

Type

Source

EventSource

null

∅

Interactions

The `Touchable Events` node takes in a global Event Source reference and will listen for events from that global reference. When it detects something happening, it will fire events depending on what happens, along with other data.

## Outputs

### OnEvent ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Fires an [Impulse](https://wiki.resonite.com/Impulses "Impulses") when the event happens.

### Hover ( [EventState](https://wiki.resonite.com/Type:EventState "Type:EventState"))

The event state that defines this hover.

### Touch ( [EventState](https://wiki.resonite.com/Type:EventState "Type:EventState"))

The event state that defines this touch.

### Point ( [float3](https://wiki.resonite.com/Type:Float3 "Type:Float3"))

The point in global transform in the world the user's cursor is at on the surface of the button during any of this node's Impulses.
Also see: [Coordinate spaces](https://wiki.resonite.com/Coordinate_spaces "Coordinate spaces")

### Tip ( [float3](https://wiki.resonite.com/Type:Float3 "Type:Float3"))

The tip of the touchable.

### Source ( [Component](https://wiki.resonite.com/Component "Component"))

The source of the button press.

When using the laser on the button, this returns with `RelayTouchSource`.

When physically pressing the button, this returns with `TipTouchSource`.

## Globals

### EventSource ( [TouchEventRelay](https://wiki.resonite.com/Component:TouchEventRelay "Component:TouchEventRelay"))

The TouchEventRelay component to read events from.

## See also

[ProtoFlux:ButtonEvents](https://wiki.resonite.com/ProtoFlux:ButtonEvents "ProtoFlux:ButtonEvents")

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:TouchableEvents&oldid=113684](https://wiki.resonite.com/index.php?title=ProtoFlux:TouchableEvents&oldid=113684)"

Contents