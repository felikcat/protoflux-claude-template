# ProtoFlux:IndirectWrite

> Source: https://wiki.resonite.com/ProtoFlux:IndirectWrite

Indirect Write

\*

OnWritten

Variable

OnFail

Value

Indirect

Indirect writes can be commonly found in legacy content that has been migrated from other platforms.
Indirect writes take Variable ( [Variable](https://wiki.resonite.com/Type:IVariable%602 "Type:IVariable`2")) as an input, and the type that Variable wraps will determine what Value (Generic) will take as a value. The node will then write Value (Generic) to the field Variable ( [Variable](https://wiki.resonite.com/Type:IVariable%602 "Type:IVariable`2")) wraps.

Indirect Writes are a way to change a specified value without driving it. Instead you can use Indirect Writes to change a value in a similar fashion to changing the value through the inspector. Using Indirect Writes helps with performance too, since the values provided to the node only evaluate for one game tick while the node is being impulsed vs a driver which evaluates every game tick. This can also be used to reduce the amount of times code is evaluated. If you have to search the entire root for your code to find a slot and then do an operation, using Indirect Writes with your operations will help with performance since you're only searching once and not every single game tick.

[Variables](https://wiki.resonite.com/Type:IVariable%602 "Type:IVariable`2") for Indirect Writes can be made using a [Field As Variable](https://wiki.resonite.com/ProtoFlux:Field_As_Variable "ProtoFlux:Field As Variable") which can wrap any [type](https://wiki.resonite.com/Category:Type "Category:Type") (Generic). [Variables](https://wiki.resonite.com/Type:IVariable%602 "Type:IVariable`2") can also be made by dragging a source of the same wrapped type (ex:Source<String> -> Variable<String>) into any variable input and it will make a [special converter](https://wiki.resonite.com/ProtoFlux:Reference_To_Output "ProtoFlux:Reference To Output") to connect them. This can be multiplexed using [Multiplexing](https://wiki.resonite.com/ProtoFlux:Multiplex "ProtoFlux:Multiplex") for using multiple variables into the same input on Indirect Writes. Multiplexing the inputs on Indirect Writes can be useful in modifying a list of variables during a [For](https://wiki.resonite.com/ProtoFlux:For "ProtoFlux:For") or [While](https://wiki.resonite.com/ProtoFlux:While "ProtoFlux:While") loop.

## Indirect Write or Write?

The difference between a [Write](https://wiki.resonite.com/ProtoFlux:Write "ProtoFlux:Write") node and an Indirect Write is in how they reference the variable they affect.  In a Write node, what is called a [Global](https://wiki.resonite.com/index.php?title=Global&action=edit&redlink=1 "Global (page does not exist)") is used to hold the variable, and this reference is only evaluated when the Protoflux starts executing.  Therefore, code that changes the variable for a normal Write during its execution will have no effect.

In contrast, an Indirect Write node uses a normal input for its variable, which is evaluated whenever the node is called.  This allows for the variable to be programmatically changed during the flow of execution, such as via a [multiplexer](https://wiki.resonite.com/ProtoFlux:Multiplex "ProtoFlux:Multiplex") with an indeterminate number of possible inputs.

In short, if you're writing to a static variable stick with normal [Write](https://wiki.resonite.com/ProtoFlux:Write "ProtoFlux:Write"), while if your code might change the variable you're writing to during execution use Indirect Write instead.

## Inputs

### \\* ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Call this to write the value.

### Variable ( [Variable](https://wiki.resonite.com/Type:IVariable%602 "Type:IVariable`2") Generic)

The [Variable](https://wiki.resonite.com/Type:IVariable%602 "Type:IVariable`2") to write to.

### Value (Generic)

[Value](https://wiki.resonite.com/Category:Type "Category:Type") to write to the value being wrapped by Variable [Variable](https://wiki.resonite.com/Type:IVariable%602 "Type:IVariable`2")

## Outputs

### OnWritten ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

sends an impulse after \* ( [Call](https://wiki.resonite.com/Impulses "Impulses")) has been impulsed and the value has been written.

### OnFail ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

sends an impulse after \* ( [Call](https://wiki.resonite.com/Impulses "Impulses")) has been impulsed and the value wasn't able to be written due to a missing target or the variable not wrapping a valid [IValue\`1](https://wiki.resonite.com/Type:IValue%601 "Type:IValue`1")

## Examples

- [How to use multiplexing on an indirect node type to switch variables using a for loop.](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=Protoflux_example_multiplexing_variables.webp "File:Protoflux example multiplexing variables.webp")

How to use multiplexing on an indirect node type to switch variables using a for loop.

- [How to use a source to make an indirect variable.](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=Protoflux_example_source_to_indirect_variable.webp "File:Protoflux example source to indirect variable.webp")

How to use a source to make an indirect variable.

- [![A basic setup for making an Indirect Write write to a field shown in the inspector.](https://wiki.resonite.com/images/thumb/5/52/ProtoFlux_Indirect_Write_Example_Basic.jpg/480px-ProtoFlux_Indirect_Write_Example_Basic.jpg)](https://wiki.resonite.com/File:ProtoFlux_Indirect_Write_Example_Basic.jpg "A basic setup for making an Indirect Write write to a field shown in the inspector.")

A basic setup for making an Indirect Write write to a field shown in the inspector.


Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:IndirectWrite&oldid=110061](https://wiki.resonite.com/index.php?title=ProtoFlux:IndirectWrite&oldid=110061)"

Contents