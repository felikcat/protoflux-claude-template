# ProtoFlux:DestroySlotChildren

> Source: https://wiki.resonite.com/ProtoFlux:DestroySlotChildren

Destroy Slot Children

\*

Next

Instance

PreserveAssets

SendDestroyingEvent

Slots

Remove all children of the provided Instance ( [Slot](https://wiki.resonite.com/Slot "Slot")).

## Inputs

### \\* ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Call to destroy the children slots of Instance ( [Slot](https://wiki.resonite.com/Slot "Slot"))

### Instance ( [Slot](https://wiki.resonite.com/Slot "Slot"))

The slot to destroy all the children for.

### PreserveAssets ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Whether or not the assets associated with the children of the provided Instance ( [Slot](https://wiki.resonite.com/Slot "Slot")) should stay or be instantly discarded

### SendDestroyingEvent ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Whether or not to send a destroying event of the children slots to other nodes like [On Destroying](https://wiki.resonite.com/ProtoFlux:On_Destroying "ProtoFlux:On Destroying")

## Outputs

### Next ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Sends an Impulse after \* ( [Call](https://wiki.resonite.com/Impulses "Impulses")) is called and Instance ( [Slot](https://wiki.resonite.com/Slot "Slot"))'s children has been destroyed. will not fire if Instance ( [Slot](https://wiki.resonite.com/Slot "Slot")) is null.

## Examples

- [A button hooked up to destroy a huge list of children of slot using Destroy Children](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=ProtoFlux_example_destroy_slot_children_1.webp "File:ProtoFlux example destroy slot children 1.webp")

A button hooked up to destroy a huge list of children of slot using Destroy Children

- [The aftermath of pressing the button.](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=ProtoFlux_example_destroy_slot_children_2.webp "File:ProtoFlux example destroy slot children 2.webp")

The aftermath of pressing the button.


Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:DestroySlotChildren&oldid=109675](https://wiki.resonite.com/index.php?title=ProtoFlux:DestroySlotChildren&oldid=109675)"

Contents