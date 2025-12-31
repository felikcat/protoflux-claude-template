# ProtoFlux:SetParent

> Source: https://wiki.resonite.com/ProtoFlux:SetParent

Set Parent Slot

\*

Next

Instance

NewParent

PreserveGlobalPosition

Slots

Sets the parent of Instance ( [Slot](https://wiki.resonite.com/Slot "Slot")).

## Inputs

### \\* ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Set the parent of Instance ( [Slot](https://wiki.resonite.com/Slot "Slot")) to NewParent ( [Slot](https://wiki.resonite.com/Slot "Slot"))

### Instance ( [Slot](https://wiki.resonite.com/Slot "Slot"))

The slot to set the parent of.

### NewParent ( [Slot](https://wiki.resonite.com/Slot "Slot"))

The slot to set the parent of Instance ( [Slot](https://wiki.resonite.com/Slot "Slot")) to.

### PreserveGlobalPosition ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Whether or not to keep the values for Instance ( [Slot](https://wiki.resonite.com/Slot "Slot"))'s local transforms or to keep it in the same place visually.

## Outputs

### Next ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Sends an impulse when Instance ( [Slot](https://wiki.resonite.com/Slot "Slot")) is sucessfully parented to NewParent ( [Slot](https://wiki.resonite.com/Slot "Slot")), or if NewParent ( [Slot](https://wiki.resonite.com/Slot "Slot")) is null it will set it to the Root Slot of the World.

## Examples

- [An example of the slot "Foo" setting it's parent slot set to "Bar" from "Foo2".](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=ProtoFlux_Example_Set_Parent_Slot "File:ProtoFlux Example Set Parent Slot")

An example of the slot "Foo" setting it's parent slot set to "Bar" from "Foo2".


Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:SetParent&oldid=110715](https://wiki.resonite.com/index.php?title=ProtoFlux:SetParent&oldid=110715)"

Contents