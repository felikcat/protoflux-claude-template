# ProtoFlux:ElementExists

> Source: https://wiki.resonite.com/ProtoFlux:ElementExists

Element Exists

Element

\*

Elements

The `Element Exists` node takes in a [world element](https://wiki.resonite.com/Type:IWorldElement "Type:IWorldElement") and returns if that element exists in the world currently. This node will not update in the way you think it does, due to the fact that destroying slots in a world does not remove them immediately, instead they are still referenced in the [Assets Slot](https://wiki.resonite.com/Assets_(Slot) "Assets (Slot)") waiting to be [garbage collected](https://en.wikipedia.org/wiki/Garbage_collection_(computer_science)) (and will still say `true`). Once that slot has been garbage collected, the reference will be removed and this node will say `false`.

## Inputs

### Element ( [IWorldElement](https://wiki.resonite.com/Type:IWorldElement "Type:IWorldElement"))

The world element in question.

## Outputs

### \\* ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Returns if this element exists in this world.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:ElementExists&oldid=109709](https://wiki.resonite.com/index.php?title=ProtoFlux:ElementExists&oldid=109709)"

Contents