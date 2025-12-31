# ProtoFlux:DuplicateSlot

> Source: https://wiki.resonite.com/ProtoFlux:DuplicateSlot

Duplicate Slot

\*

Next

Template

Duplicate

OverrideParent

Slots

The **Duplicate Slot** node makes a copy of a [slot](https://wiki.resonite.com/Slot "Slot") and exposes the duplicated slot with the output called `Duplicate` which can be used for any nodes that accept the [slot](https://wiki.resonite.com/Slot "Slot") type.

This node can take an overriding parent as an input for the duplicated slot. This acts similarly to the [Set Parent](https://wiki.resonite.com/ProtoFlux:Set_Parent "ProtoFlux:Set Parent") node (with `PreserveGlobalPosition` enabled, which is default on that node) without needing the extra node.

## Inputs

### \\* ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Call this to write the value.

### Template ( [Slot](https://wiki.resonite.com/Slot "Slot"))

The slot to make a duplicate of.

### OverrideParent ( [Slot](https://wiki.resonite.com/Slot "Slot"))

The slot to place the duplicated slot under.

## Outputs

### Next ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Will fire after Instance ( [Slot](https://wiki.resonite.com/Slot "Slot")) has been duplicated due to \* ( [Call](https://wiki.resonite.com/Impulses "Impulses")) being impulsed.

### Duplicate ( [Slot](https://wiki.resonite.com/Slot "Slot"))

The duplicate of Instance ( [Slot](https://wiki.resonite.com/Slot "Slot")). Will only exist during the Next ( [Continuation](https://wiki.resonite.com/Impulses "Impulses")) Impulse context.

## Examples

- [Example of how to use a duplicate slot with a template, to make a vending-machine esque item button.](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=Protoflux_example_duplicate_slot.webp "File:Protoflux example duplicate slot.webp")

Example of how to use a duplicate slot with a template, to make a vending-machine esque item button.


Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:DuplicateSlot&oldid=109685](https://wiki.resonite.com/index.php?title=ProtoFlux:DuplicateSlot&oldid=109685)"

Contents