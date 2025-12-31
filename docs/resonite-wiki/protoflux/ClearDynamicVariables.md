# ProtoFlux:ClearDynamicVariables

> Source: https://wiki.resonite.com/ProtoFlux:ClearDynamicVariables

Clear Dynamic Variables

\*

OnNotFound

Target

OnCleared

SpaceName

ClearedCount

Dynamic

The `Clear Dynamic Variables` node takes in a [slot](https://wiki.resonite.com/Slot "Slot") hierarchy and a [string](https://wiki.resonite.com/Type:String "Type:String") literal path of the [dynamic space](https://wiki.resonite.com/Component:DynamicVariableSpace "Component:DynamicVariableSpace") name. For more information, see [Dynamic Variables](https://wiki.resonite.com/Dynamic_Variables "Dynamic Variables").

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

Keep in mind that the top most output is **OnNotFound**. This can be confusing (especially if you're not paying attention when connecting nodes) when the code fires and nothing happens.


## Inputs

### \\* ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Calls an impulse to clear all dynamic variables from a given dynamic space.

### Target ( [Slot](https://wiki.resonite.com/Slot "Slot"))

The slot hierarchy for this node to look through.

### SpaceName ( [string](https://wiki.resonite.com/Type:String "Type:String"))

The dynamic space name to find and clear out the dynamic variables from.

## Outputs

### OnNotFound ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Fires when the path is incorrect or there is nothing to find in the given slot hierarchy.

### OnCleared ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Fires when the dynamic space name is found and all dynamic variables under that name is removed.

### ClearedCount ( [int](https://wiki.resonite.com/Type:Int "Type:Int"))

Returns the number of dynamic variables that have been removed by this node.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:ClearDynamicVariables&oldid=111817](https://wiki.resonite.com/index.php?title=ProtoFlux:ClearDynamicVariables&oldid=111817)"

Contents