# ProtoFlux:ClearDynamicVariablesOfType

> Source: https://wiki.resonite.com/ProtoFlux:ClearDynamicVariablesOfType

Clear Dynamic Variables Of Type

\*

OnNotFound

Target

OnCleared

SpaceName

ClearedCount

Dynamic

The `Clear Dynamic Variables Of Type` node takes in a [slot](https://wiki.resonite.com/Slot "Slot") hierarchy and a [string](https://wiki.resonite.com/Type:String "Type:String") literal path of the [dynamic space](https://wiki.resonite.com/Component:DynamicVariableSpace "Component:DynamicVariableSpace") name. For more information, see [Dynamic Variables](https://wiki.resonite.com/Dynamic_Variables "Dynamic Variables"). This node then uses the selected type and searches through that hierarchy and only removes the dynamic variables of that matching type.

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

Keep in mind that the top most output is **OnNotFound**. This can be confusing (especially if you're not paying attention when connecting nodes) when the code fires and nothing happens.


## Inputs

### \\* ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Calls an impulse to clear all dynamic variables of that type from a given dynamic space.

### Target ( [Slot](https://wiki.resonite.com/Slot "Slot"))

The slot hierarchy for this node to look through.

### SpaceName ( [string](https://wiki.resonite.com/Type:String "Type:String"))

The dynamic space name to find and clear out the dynamic variables of declared type from.

## Outputs

### OnNotFound ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Fires when the path is incorrect or there is nothing to find in the given slot hierarchy that matches that type.

### OnCleared ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Fires when the dynamic space name is found and all dynamic variables of that type under that name is removed.

### ClearedCount ( [int](https://wiki.resonite.com/Type:Int "Type:Int"))

Returns the number of dynamic variables of that type that have been removed by this node.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:ClearDynamicVariablesOfType&oldid=111818](https://wiki.resonite.com/index.php?title=ProtoFlux:ClearDynamicVariablesOfType&oldid=111818)"

Contents