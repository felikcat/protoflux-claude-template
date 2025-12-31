# ProtoFlux:DynamicVariableInputWithEvents

> Source: https://wiki.resonite.com/ProtoFlux:DynamicVariableInputWithEvents

DynVar Input with Events

DetectingUser

OnSpaceLinked

OnSpaceUnlinked

Value

HasValue

VariableName

null

∅

Dynamic

Dynamic Variable Input with Events is a ProtoFlux node that is able to read from a [dynamic variable space](https://wiki.resonite.com/Component:DynamicVariableSpace "Component:DynamicVariableSpace") the same as a [Dynamic Variable Driver Component](https://wiki.resonite.com/Component:DynamicValueVariableDriver "Component:DynamicValueVariableDriver") does, by reading a dynamic variable value using its own slot as a read point. To see how dynamic variables are created and read, see [Dynamic Variables](https://wiki.resonite.com/Dynamic_Variables "Dynamic Variables"). If you want to change the path dynamically, use [Read Dynamic Variable](https://wiki.resonite.com/ProtoFlux:Read_Dynamic_Variable "ProtoFlux:Read Dynamic Variable") but without providing a slot to Source ( [Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")).

This node has the added benefit of firing events when a slot with a dynamic variable has been moved, created, or deleted. This is called linking or unlinking and this node will fire these events when detected. This node also takes in a detecting user, in cases where you want to check if a user has detected the slots with variables available.

![](https://wiki.resonite.com/images/c/c1/SuggestionIcon.svg)

If you want a simplier node that just gives the value, use [Dynamic Variable Input](https://wiki.resonite.com/ProtoFlux:Dynamic_Variable_Input "ProtoFlux:Dynamic Variable Input") instead.


## Inputs

### DetectingUser ( [User](https://wiki.resonite.com/User "User"))

The user that is listening for slots (containing the dynamic variable) that suddenly have been moved, created, or deleted.

## Outputs

### OnSpaceLinked ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Fires when a slot with a matching dynamic variable name has been detected and is ready to be used or read from.

### OnSpaceUnlinked ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Fires when a slot with a matching dynamic variable name has been moved or removed in some way and is now no longer being detected.

### Value (Generic)

Outputs the value of the dynamic variable with the type of `Value` and a variable name of `VariableName`

### HasValue ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Outputs whether or not a variable of `VariableName` could be found from this node.

## Globals

### VariableName ( [String](https://wiki.resonite.com/Type:String "Type:String"))

The name to read for a dynamic variable with. To see how the name of a dynamic variable can be written, including how it can vary wildly, see [Dynamic Variables](https://wiki.resonite.com/Dynamic_Variables "Dynamic Variables")

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:DynamicVariableInputWithEvents&oldid=111822](https://wiki.resonite.com/index.php?title=ProtoFlux:DynamicVariableInputWithEvents&oldid=111822)"

Contents