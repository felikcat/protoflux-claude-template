# ProtoFlux:ButtonEvents

> Source: https://wiki.resonite.com/ProtoFlux:ButtonEvents

Button Events

Pressed

Pressing

Released

HoverEnter

HoverStay

HoverLeave

Source

GlobalPoint

LocalPoint

NormalizedPoint

Button

null

∅

Interactions

The `Button Events` node takes in a global [IButton](https://wiki.resonite.com/Type:IButton "Type:IButton") reference and will listen for events from that global reference. When it detects something happening, it will fire events depending on what happens, along with other data.

You can use this node with [UI Buttons](https://wiki.resonite.com/Component:Button "Component:Button"), [Touch Buttons](https://wiki.resonite.com/Component:TouchButton "Component:TouchButton"), [Physical Buttons](https://wiki.resonite.com/Component:PhysicalButton "Component:PhysicalButton"), [Context Menu](https://wiki.resonite.com/Context_menu "Context menu") Buttons, or even a custom button you add as a component onto a [Slot](https://wiki.resonite.com/Slot "Slot") or object, like a box.

## Outputs

### Pressed ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Sends an Impulse when the button in Global: IButton is pressed down

### Pressing ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Sends an Impulse every game update while the button in Global: IButton is being held down

### Released ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Sends an Impulse when the button in Global: IButton is released

### HoverEnter ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Sends an Impulse a cursor/laser is brought on top of the button in Global: IButton (TODO: Does this include touching? (Ex: Physical buttons))

### HoverStay ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Sends an Impulse every game update while the button in Global: IButton is being currently being hovered over (TODO: Does this include touching? (Ex: Physical buttons))

### HoverLeave ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Sends an Impulse a cursor/laser leaves being on top of the button in Global: IButton (TODO: Does this include touching? (Ex: Physical buttons))

### Source ( [Component](https://wiki.resonite.com/Component "Component"))

The source of the button press.

When using the laser on the button, this returns with `RelayTouchSource`.

When physically pressing the button, this returns with `TipTouchSource`.

### GlobalPoint ( [float3](https://wiki.resonite.com/Type:Float3 "Type:Float3"))

The point in global transform in the world the user's cursor is at on the surface of the button during any of this node's Impulses
Example: Useful for a splash of particles where the user clicked like a click effect
Also see: [Coordinate spaces](https://wiki.resonite.com/Coordinate_spaces "Coordinate spaces")

### LocalPoint ( [float3](https://wiki.resonite.com/Type:Float3 "Type:Float3"))

The point in UIX pixels within the button's local [RectTransform](https://wiki.resonite.com/RectTransform_(Component) "RectTransform (Component)") the user's cursor is at during any of this node's Impulses
Also see: [Coordinate spaces](https://wiki.resonite.com/Coordinate_spaces "Coordinate spaces")

### NormalizedPoint ( [float2](https://wiki.resonite.com/Type:Float2 "Type:Float2"))

The point from 0 to 1 in both the x and y channels within the button's local [RectTransform](https://wiki.resonite.com/RectTransform_(Component) "RectTransform (Component)") the user's cursor is at during any of this node's Impulses.
Also see: [Coordinate spaces](https://wiki.resonite.com/Coordinate_spaces "Coordinate spaces")

## Globals

### Button ( [IButton](https://wiki.resonite.com/Type:IButton "Type:IButton"))

[IButton](https://wiki.resonite.com/Type:IButton "Type:IButton") to read events from.

## Examples

[![](https://wiki.resonite.com/images/thumb/3/3f/EventTypeDetectionExample.png/300px-EventTypeDetectionExample.png)](https://wiki.resonite.com/File:EventTypeDetectionExample.png) Detecting if an event is laser or physical

- [Button Events being used to make a sound play.](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=ProtoFlux_example_button_events "File:ProtoFlux example button events")

Button Events being used to make a sound play.


## See also

[ProtoFlux:TouchableEvents](https://wiki.resonite.com/ProtoFlux:TouchableEvents "ProtoFlux:TouchableEvents")

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:ButtonEvents&oldid=113683](https://wiki.resonite.com/index.php?title=ProtoFlux:ButtonEvents&oldid=113683)"

Contents