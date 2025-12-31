# ProtoFlux:IndirectWriteLatch

> Source: https://wiki.resonite.com/ProtoFlux:IndirectWriteLatch

Indirect Write Latch

Set

OnSet

Reset

OnReset

Variable

OnFail

SetValue

ResetValue

Indirect

Indirect write latches can be commonly found in legacy content that has been migrated from other platforms.
Indirect write latches take Variable ( [Variable](https://wiki.resonite.com/Type:IVariable%602 "Type:IVariable`2")) as an input, and the type that Variable wraps will determine what SetValue (Generic) and ResetValue (Generic) will take as a value. The set and reset value inputs will never take different types from each other.

Indirect Write Latches are a way to change a specified value without driving it. Instead you can use Indirect Write Latches to change a value in a similar fashion to changing the value through the inspector. Using Indirect Write Latches helps with performance too, since the values provided to the node only evaluate for one game tick while the node is being impulsed vs a driver which evaluates every game tick. This can also be used to reduce the amount of times code is evaluated. If you have to search the entire root for your code to find a slot and then do an operation, using Indirect Write Latches with your operations will help with performance since you're only searching once and not every single game tick.

[Variables](https://wiki.resonite.com/Type:IVariable%602 "Type:IVariable`2") for Indirect Write Latches can be made using a [Field As Variable](https://wiki.resonite.com/ProtoFlux:Field_As_Variable "ProtoFlux:Field As Variable") which can wrap any [type](https://wiki.resonite.com/Category:Type "Category:Type") (Generic). [Variables](https://wiki.resonite.com/Type:IVariable%602 "Type:IVariable`2") can also be made by dragging a source of the same wrapped type (ex:Source<String> -> Variable<String>) into any variable input and it will make a [special converter](https://wiki.resonite.com/ProtoFlux:Reference_To_Output "ProtoFlux:Reference To Output") to connect them. This can be multiplexed using [Multiplexing](https://wiki.resonite.com/ProtoFlux:Multiplex "ProtoFlux:Multiplex") for using multiple variables into the same input on Indirect Write Latches. Multiplexing the inputs on Indirect Write Latches can be useful in modifying a list of variables during a [For](https://wiki.resonite.com/ProtoFlux:For "ProtoFlux:For") or [While](https://wiki.resonite.com/ProtoFlux:While "ProtoFlux:While") loop.

## Inputs

### Reset ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Call this to set the value being wrapped by Variable ( [Variable](https://wiki.resonite.com/Type:IVariable%602 "Type:IVariable`2") Generic) to the ResetValue (Generic) input.

### Set ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Call this to set the value being wrapped by Variable ( [Variable](https://wiki.resonite.com/Type:IVariable%602 "Type:IVariable`2") Generic) to the SetValue (Generic) input.

### Variable ( [Variable](https://wiki.resonite.com/Type:IVariable%602 "Type:IVariable`2") Generic)

The [Variable](https://wiki.resonite.com/Type:IVariable%602 "Type:IVariable`2") to write to.

### SetValue (Generic)

[Value](https://wiki.resonite.com/Category:Type "Category:Type") to write to the value wrapped by Variable ( [Variable](https://wiki.resonite.com/Type:IVariable%602 "Type:IVariable`2") Generic) upon calling Set ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

### ResetValue (Generic)

[Value](https://wiki.resonite.com/Category:Type "Category:Type") to write to the value wrapped by Variable ( [Variable](https://wiki.resonite.com/Type:IVariable%602 "Type:IVariable`2") Generic) upon calling Reset ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

## Outputs

### OnSet ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

sends an impulse after SetValue ( [Call](https://wiki.resonite.com/Impulses "Impulses")) has been impulsed and the value wrapped by Variable ( [Variable](https://wiki.resonite.com/Type:IVariable%602 "Type:IVariable`2") Generic) has been set to SetValue (Generic).

### OnReset ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

sends an impulse after ResetValue ( [Call](https://wiki.resonite.com/Impulses "Impulses")) has been impulsed and the value wrapped by Variable ( [Variable](https://wiki.resonite.com/Type:IVariable%602 "Type:IVariable`2") Generic) has been set to ResetValue (Generic).

### OnFail ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

sends an impulse after either ResetValue ( [Call](https://wiki.resonite.com/Impulses "Impulses")) or SetValue ( [Call](https://wiki.resonite.com/Impulses "Impulses")) has been impulsed and the value wasn't able to be written due to a missing target or the variable not wrapping a valid [IValue\`1](https://wiki.resonite.com/Type:IValue%601 "Type:IValue`1")

## Examples

- [How to use multiplexing on an indirect node type to switch variables using a for loop.](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=Protoflux_example_multiplexing_variables.webp "File:Protoflux example multiplexing variables.webp")

How to use multiplexing on an indirect node type to switch variables using a for loop.

- [How to use a source to make an indirect variable.](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=Protoflux_example_source_to_indirect_variable.webp "File:Protoflux example source to indirect variable.webp")

How to use a source to make an indirect variable.

- [How to use a simple indirect write latch setup.](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=Protoflux_example_indirect_write_latch.webp "File:Protoflux example indirect write latch.webp")

How to use a simple indirect write latch setup.


Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:IndirectWriteLatch&oldid=110063](https://wiki.resonite.com/index.php?title=ProtoFlux:IndirectWriteLatch&oldid=110063)"

Contents