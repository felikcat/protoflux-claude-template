# ProtoFlux:DynamicVariableInput

> Source: https://wiki.resonite.com/ProtoFlux:DynamicVariableInput

DynVar Input

Value

HasValue

VariableName

null

∅

Dynamic

Dynamic Variable Input is a ProtoFlux node that is able to read from a [dynamic variable space](https://wiki.resonite.com/Component:DynamicVariableSpace "Component:DynamicVariableSpace") the same as a [Dynamic Variable Driver Component](https://wiki.resonite.com/Component:DynamicValueVariableDriver "Component:DynamicValueVariableDriver") does, by reading a dynamic variable value using its own slot as a read point. To see how dynamic variables are created and read, see [Dynamic Variables](https://wiki.resonite.com/Dynamic_Variables "Dynamic Variables"). If you want to change the path dynamically, use [Read Dynamic Variable](https://wiki.resonite.com/ProtoFlux:Read_Dynamic_Variable "ProtoFlux:Read Dynamic Variable") but without providing a slot to Source ( [Slot](https://wiki.resonite.com/Type:Slot "Type:Slot"))

![](https://wiki.resonite.com/images/c/c1/SuggestionIcon.svg)

If you want more control on when a slot is linked/unlinked, use [Dynamic Variable Input with Events](https://wiki.resonite.com/ProtoFlux:Dynamic_Variable_Input_With_Events "ProtoFlux:Dynamic Variable Input With Events") instead.


## Outputs

### Value (Generic)

Outputs the value of the dynamic variable with the type of `Value` and a variable name of `VariableName`

### HasValue ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Outputs whether or not a variable of `VariableName` could be found from this node.

## Globals

### VariableName ( [String](https://wiki.resonite.com/Type:String "Type:String"))

The name to read for a dynamic variable with. To see how the name of a dynamic variable can be written, including how it can vary wildly, see [Dynamic Variables](https://wiki.resonite.com/Dynamic_Variables "Dynamic Variables")

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:DynamicVariableInput&oldid=111821](https://wiki.resonite.com/index.php?title=ProtoFlux:DynamicVariableInput&oldid=111821)"

Contents