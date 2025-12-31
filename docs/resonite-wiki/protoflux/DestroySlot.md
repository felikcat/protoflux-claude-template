# ProtoFlux:DestroySlot

> Source: https://wiki.resonite.com/ProtoFlux:DestroySlot

Destroy Slot

\*

Next

Instance

PreserveAssets

SendDestroyingEvent

Slots

Destroys the Provided Instance ( [Slot](https://wiki.resonite.com/Slot "Slot")) when \* ( [Call](https://wiki.resonite.com/Impulses "Impulses")) is called.

## Inputs

### \\* ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Call to destroy Instance ( [Slot](https://wiki.resonite.com/Slot "Slot"))

### Instance ( [Slot](https://wiki.resonite.com/Slot "Slot"))

The slot to destroy

### PreserveAssets ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Whether or not the assets associated with the provided Instance ( [Slot](https://wiki.resonite.com/Slot "Slot")) should stay or be instantly discarded

### SendDestroyingEvent ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Whether or not to send a destroying event to other nodes like [On Destroying](https://wiki.resonite.com/ProtoFlux:On_Destroying "ProtoFlux:On Destroying")

## Outputs

### Next ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Sends an Impulse after \* ( [Call](https://wiki.resonite.com/Impulses "Impulses")) is called and Instance ( [Slot](https://wiki.resonite.com/Slot "Slot")) has been destroyed. will not fire if Instance ( [Slot](https://wiki.resonite.com/Slot "Slot")) is null.

## Examples

- [A button that is hooked up to destroy a box and would display "Destroyed!". currently displays "Not pressed.".](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=ProtoFlux_example_destroy_slot_1.webp "File:ProtoFlux example destroy slot 1.webp")

A button that is hooked up to destroy a box and would display "Destroyed!". currently displays "Not pressed.".

- [The result of the code, where the box destroyed and the button displays "Destroyed!".](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=ProtoFlux_example_destroy_slot_2.webp "File:ProtoFlux example destroy slot 2.webp")

The result of the code, where the box destroyed and the button displays "Destroyed!".


Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:DestroySlot&oldid=109673](https://wiki.resonite.com/index.php?title=ProtoFlux:DestroySlot&oldid=109673)"

Contents