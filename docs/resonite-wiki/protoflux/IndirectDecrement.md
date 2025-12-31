# ProtoFlux:IndirectDecrement

> Source: https://wiki.resonite.com/ProtoFlux:IndirectDecrement

Indirect Decrement

\*

OnWritten

Variable

OnFail

Indirect

Indirect decrements can be commonly found in legacy content that has been migrated from other platforms.
Indirect decrements take Variable ( [Variable](https://wiki.resonite.com/Type:IVariable%602 "Type:IVariable`2")) as an input, and will decrease the value that is wrapped by Variable ( [Variable](https://wiki.resonite.com/Type:IVariable%602 "Type:IVariable`2")) by one.

Indirect Decrements are a way to change a specified value without driving it. Instead you can use Indirect Decrements to change a value in a similar fashion to changing the value through the inspector. Using Indirect Decrements helps with performance too, since the values provided to the node only evaluate for one game tick while the node is being impulsed vs a driver which evaluates every game tick. This can also be used to reduce the amount of times code is evaluated. If you have to search the entire root for your code to find a slot and then do an operation, using Indirect Decrements with your operations will help with performance since you're only searching once and not every single game tick.

![](https://wiki.resonite.com/images/d/dd/InformationIcon.svg)

Keep in mind this node will only work if given variables that can be decremented. Trying to decrement a non numeric value like a [Boolean](https://wiki.resonite.com/Type:Bool "Type:Bool") or an [Enum](https://wiki.resonite.com/Category:Enums "Category:Enums") will not work.


[Variables](https://wiki.resonite.com/Type:IVariable%602 "Type:IVariable`2") for Indirect Decrements can be made using a [Field As Variable](https://wiki.resonite.com/ProtoFlux:Field_As_Variable "ProtoFlux:Field As Variable") which can wrap any [type](https://wiki.resonite.com/Category:Type "Category:Type") (Generic). [Variables](https://wiki.resonite.com/Type:IVariable%602 "Type:IVariable`2") can also be made by dragging a source of the same wrapped type (ex:Source<String> -> Variable<String>) into any variable input and it will make a [special converter](https://wiki.resonite.com/ProtoFlux:Reference_To_Output "ProtoFlux:Reference To Output") to connect them. This can be multiplexed using [Multiplexing](https://wiki.resonite.com/ProtoFlux:Multiplex "ProtoFlux:Multiplex") for using multiple variables into the same input on Indirect Decrements. Multiplexing the inputs on Indirect Decrements can be useful in modifying a list of variables during a [For](https://wiki.resonite.com/ProtoFlux:For "ProtoFlux:For") or [While](https://wiki.resonite.com/ProtoFlux:While "ProtoFlux:While") loop.

## Inputs

### \\* ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Call this to write the value.

### Variable ( [Variable](https://wiki.resonite.com/Type:IVariable%602 "Type:IVariable`2") Generic)

The [Variable](https://wiki.resonite.com/Type:IVariable%602 "Type:IVariable`2") to decrement by 1.

## Outputs

### OnWritten ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

sends an impulse after \* ( [Call](https://wiki.resonite.com/Impulses "Impulses")) has been impulsed and the value has been decremented .

### OnFail ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

sends an impulse after \* ( [Call](https://wiki.resonite.com/Impulses "Impulses")) has been impulsed and the value wasn't able to be decremented due to a missing target or the variable not wrapping a valid [IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1")

## Examples

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:IndirectDecrement&oldid=110057](https://wiki.resonite.com/index.php?title=ProtoFlux:IndirectDecrement&oldid=110057)"

Contents