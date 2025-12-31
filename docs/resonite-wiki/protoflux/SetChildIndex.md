# ProtoFlux:SetChildIndex

> Source: https://wiki.resonite.com/ProtoFlux:SetChildIndex

Set Child Index

\*

Next

Instance

Index

Slots

Sets the offset of the provided Instance ( [Slot](https://wiki.resonite.com/Slot "Slot")) in the inspector compared to others that have the same immediate parent to Index ( [Int](https://wiki.resonite.com/Types:Int "Types:Int")).

It should be noted that this node will normally update the OrderOffset of all slots adjacent to the Instance slot (i.e. having the same Parent slot as Instance) to ensure that the Instance slot gets the correct child index.

## Inputs

### \\* ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Call to set the index of Instance ( [Slot](https://wiki.resonite.com/Slot "Slot")) to Index ( [Int](https://wiki.resonite.com/Types:Int "Types:Int")).

### Instance ( [Slot](https://wiki.resonite.com/Slot "Slot"))

The slot to set the child index of.

### Index ( [Int](https://wiki.resonite.com/Types:Int "Types:Int"))

The child index to set Instance ( [Slot](https://wiki.resonite.com/Slot "Slot")) to.

## Outputs

### Next ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

sends an impulse after \* ( [Call](https://wiki.resonite.com/Impulses "Impulses")) is called and Instance ( [Slot](https://wiki.resonite.com/Slot "Slot")) has had it's index set to Index ( [Int](https://wiki.resonite.com/Types:Int "Types:Int")).

## Examples

- [An example code using set child index.](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=ProtoFlux_example_set_child_index.webp "File:ProtoFlux example set child index.webp")

An example code using set child index.


Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:SetChildIndex&oldid=110661](https://wiki.resonite.com/index.php?title=ProtoFlux:SetChildIndex&oldid=110661)"

Contents