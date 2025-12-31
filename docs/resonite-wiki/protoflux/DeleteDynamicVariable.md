# ProtoFlux:DeleteDynamicVariable

> Source: https://wiki.resonite.com/ProtoFlux:DeleteDynamicVariable

Delete Dynamic Variable

\*

OnNotFound

Target

OnDeleted

Path

Dynamic

The `Delete Dynamic Variable` node takes in a [slot](https://wiki.resonite.com/Slot "Slot") hierarchy and a [string](https://wiki.resonite.com/Type:String "Type:String") literal for the path. This will check for the [dynamic variable space](https://wiki.resonite.com/Component:DynamicVariableSpace "Component:DynamicVariableSpace"), and then the variable within, if one is found, the variable will be removed. For more information, see [Dynamic Variables](https://wiki.resonite.com/Dynamic_Variables "Dynamic Variables").

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

Keep in mind that the top most output is **OnNotFound**. This can be confusing (especially if you're not paying attention when connecting nodes) when the code fires and nothing happens.


## Inputs

### \\* ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Calls an impulse to find and delete the variable from the given hierarchy and path.

### Target ( [Slot](https://wiki.resonite.com/Slot "Slot"))

This slot hierarchy to search through.

### Path ( [string](https://wiki.resonite.com/Type:String "Type:String"))

The path to find the dynamic variable.

## Outputs

### OnNotFound ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Fires when the path is incorrect or there is nothing to find in the given slot hierarchy.

### OnDeleted ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Fires when a dynamic variable was found and deleted.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:DeleteDynamicVariable&oldid=111820](https://wiki.resonite.com/index.php?title=ProtoFlux:DeleteDynamicVariable&oldid=111820)"

Contents