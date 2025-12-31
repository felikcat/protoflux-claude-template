# ProtoFlux:WriteDynamicVariable

> Source: https://wiki.resonite.com/ProtoFlux:WriteDynamicVariable

Write Dynamic Variable

\*

OnNotFound

Target

OnSuccess

Path

OnFailed

Value

Dynamic

Write Dynamic Variable is a ProtoFlux node that is able to write to previously created dynamic variables under a slot. For more info on Dynamic Variables, see [Dynamic Variables](https://wiki.resonite.com/Dynamic_Variables "Dynamic Variables"). This node will only write to the variable if the path and type it's writing to is the same as a variable that exists. See [Dynamic Variables](https://wiki.resonite.com/Dynamic_Variables "Dynamic Variables") on how equality is determined on paths, since 2 paths with different content can still make many different variables equal.

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

Keep in mind that the top most output is **OnNotFound**. This can be confusing (especially if you're not paying attention when connecting nodes) when the code fires and nothing happens.


## Inputs

### \\* ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Call this to write the variable.

### Target ( [Slot](https://wiki.resonite.com/Type:Slot "Type:Slot"))

The slot hierarchy to search for a dynamic variable to write to.

### Path ( [String](https://wiki.resonite.com/Type:String "Type:String"))

The path for finding the available dynamic variable. To see how this influences attaching see the paragraph at the beginning of this page.

### Value (Generic)

Any type of value, reference, or object that should be written to an existing variable.

## Outputs

### OnNotFound ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Fires when the path is incorrect or there is nothing to find in the given slot hierarchy.

### OnSuccess ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Fires when `*` is fired and a variable already exists that can be written to through `Target`.

### OnFailed ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Fires when `*` is fired and the variable was found but cannot be written to. The variable was not created when this impulses.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:WriteDynamicVariable&oldid=111824](https://wiki.resonite.com/index.php?title=ProtoFlux:WriteDynamicVariable&oldid=111824)"

Contents