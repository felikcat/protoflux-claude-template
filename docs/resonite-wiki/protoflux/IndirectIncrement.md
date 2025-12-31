# ProtoFlux:IndirectIncrement

> Source: https://wiki.resonite.com/ProtoFlux:IndirectIncrement

Indirect Increment

\*

OnWritten

Variable

OnFail

Indirect

Indirect increments can be commonly found in legacy content that has been migrated from other platforms.
Indirect increments take Variable ( [Variable](https://wiki.resonite.com/Type:IVariable%602 "Type:IVariable`2")) as an input, and will increase the value that is wrapped by Variable ( [Variable](https://wiki.resonite.com/Type:IVariable%602 "Type:IVariable`2")) by one.

Indirect Increments are a way to change a specified value without driving it. Instead you can use Indirect Increments to change a value in a similar fashion to changing the value through the inspector. Using Indirect Increments helps with performance too, since the values provided to the node only evaluate for one game tick while the node is being impulsed vs a driver which evaluates every game tick. This can also be used to reduce the amount of times code is evaluated. If you have to search the entire root for your code to find a slot and then do an operation, using Indirect Increments with your operations will help with performance since you're only searching once and not every single game tick.

![](https://wiki.resonite.com/images/d/dd/InformationIcon.svg)

Keep in mind this node will only work if given variables that can be increased. Trying to increase a non numeric value like a [Boolean](https://wiki.resonite.com/Type:Bool "Type:Bool") or [Enum](https://wiki.resonite.com/Category:Enums "Category:Enums") will not work.


[Variables](https://wiki.resonite.com/Type:IVariable%602 "Type:IVariable`2") for Indirect Increments can be made using a [Field As Variable](https://wiki.resonite.com/ProtoFlux:Field_As_Variable "ProtoFlux:Field As Variable") which can wrap any [type](https://wiki.resonite.com/Category:Type "Category:Type") (Generic). [Variables](https://wiki.resonite.com/Type:IVariable%602 "Type:IVariable`2") can also be made by dragging a source of the same wrapped type (ex:Source<String> -> Variable<String>) into any variable input and it will make a [special converter](https://wiki.resonite.com/ProtoFlux:Reference_To_Output "ProtoFlux:Reference To Output") to connect them. This can be multiplexed using [Multiplexing](https://wiki.resonite.com/ProtoFlux:Multiplex "ProtoFlux:Multiplex") for using multiple variables into the same input on Indirect Increments. Multiplexing the inputs on Indirect Increments can be useful in modifying a list of variables during a [For](https://wiki.resonite.com/ProtoFlux:For "ProtoFlux:For") or [While](https://wiki.resonite.com/ProtoFlux:While "ProtoFlux:While") loop.

## Inputs

### \\* ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Call this to increase the value.

### Variable ( [Variable](https://wiki.resonite.com/Type:IVariable%602 "Type:IVariable`2") Generic)

The [Variable](https://wiki.resonite.com/Type:IVariable%602 "Type:IVariable`2") to increment by 1.

## Outputs

### OnWritten ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

sends an impulse after \* ( [Call](https://wiki.resonite.com/Impulses "Impulses")) has been impulsed and the value has been incremented .

### OnFail ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

sends an impulse after \* ( [Call](https://wiki.resonite.com/Impulses "Impulses")) has been impulsed and the value wasn't able to be incremented due to a missing target or the variable not wrapping a valid [IValue\`1](https://wiki.resonite.com/Type:IValue%601 "Type:IValue`1")

## Examples

- [How to use multiplexing on an indirect node type to switch variables using a for loop.](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=Protoflux_example_multiplexing_variables.webp "File:Protoflux example multiplexing variables.webp")

How to use multiplexing on an indirect node type to switch variables using a for loop.

- [How to use a source to make an indirect variable.](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=Protoflux_example_source_to_indirect_variable.webp "File:Protoflux example source to indirect variable.webp")

How to use a source to make an indirect variable.

- [How to use a simple indirect increment setup.](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=Protoflux_example_indirect_decrement.webp "File:Protoflux example indirect decrement.webp")

How to use a simple indirect increment setup.


Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:IndirectIncrement&oldid=110059](https://wiki.resonite.com/index.php?title=ProtoFlux:IndirectIncrement&oldid=110059)"

Contents