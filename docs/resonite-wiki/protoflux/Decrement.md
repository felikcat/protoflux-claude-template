# ProtoFlux:Decrement

> Source: https://wiki.resonite.com/ProtoFlux:Decrement

\_ \_

\*

OnWritten

OnFail

Variable

null

∅

Actions

Decrements take Variable ( [Variable](https://wiki.resonite.com/Type:IVariable%602 "Type:IVariable`2") Pseudo-generic) as a global, and will decrease the value that Variable ( [Variable](https://wiki.resonite.com/Type:IVariable%602 "Type:IVariable`2") Pseudo-generic) points to by 1.

![](https://wiki.resonite.com/images/d/dd/InformationIcon.svg)

Keep in mind this node will only work if given variables that can be decremented. Trying to decrement a non numeric value like a [Boolean](https://wiki.resonite.com/Type:Bool "Type:Bool") or an [Enum](https://wiki.resonite.com/Category:Enums "Category:Enums") will not work.


Decrements are a way to change a specified value without driving it. Instead you can use Decrements to change a value in a similar fashion to changing the value through the inspector. Using Decrements helps with performance too, since the values provided to the node only evaluate for one game tick while the node is being impulsed vs a driver which evaluates every game tick. This can also be used to reduce the amount of times code is evaluated. If you have to search the entire root for your code to find a slot and then do an operation, using Decrements with your operations will help with performance since you're only searching once and not every single game tick.

When it comes to Decrements, you can drag any matching [typed](https://wiki.resonite.com/Category:Type "Category:Type") source onto the Variable field to set that as the variable target. When you want to write to a [Local Variable Store](https://wiki.resonite.com/ProtoFlux:Local "ProtoFlux:Local"), [Data Model Variable Store](https://wiki.resonite.com/ProtoFlux:Data_Model_Store "ProtoFlux:Data Model Store"), or a [Store Variable Store](https://wiki.resonite.com/ProtoFlux:Store "ProtoFlux:Store"), you can grab the Variable field on Decrements nodes and then choose the one you want in your context menu. This can save considerable time spent trying to find the type you want in another node menu.

![](https://wiki.resonite.com/images/c/c1/SuggestionIcon.svg)

If you just need to subtract 1 to your [value](https://wiki.resonite.com/Value_Type "Value Type") using pure data, use the [Value Dec](https://wiki.resonite.com/ProtoFlux:Value_Dec "ProtoFlux:Value Dec") node instead.

If you need to subtract more than 1 from your [value](https://wiki.resonite.com/Value_Type "Value Type"), use the [Sub](https://wiki.resonite.com/ProtoFlux:Sub "ProtoFlux:Sub") node instead.

## Inputs

### \\* ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Call this to write the value.

## Outputs

### OnWritten ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

sends an impulse after \* ( [Call](https://wiki.resonite.com/Impulses "Impulses")) has been impulsed and the value pointed to by Variable ( [Variable](https://wiki.resonite.com/Type:IVariable%602 "Type:IVariable`2") Pseudo-generic) has been decremented.

### OnFail ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

sends an impulse after \* ( [Call](https://wiki.resonite.com/Impulses "Impulses")) has been impulsed and the value wasn't able to be decremented due to a missing target or Variable ( [Variable](https://wiki.resonite.com/Type:IVariable%602 "Type:IVariable`2") Pseudo-generic) not pointing to a valid [IValue\`1](https://wiki.resonite.com/Type:IValue%601 "Type:IValue`1").

## Globals

### Variable ( [Variable](https://wiki.resonite.com/Type:IVariable%602 "Type:IVariable`2") Pseudo-generic)

The numeric [Variable](https://wiki.resonite.com/Type:IVariable%602 "Type:IVariable`2") to decrement by 1.

## Examples

- [How to use a simple decrement setup.](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=Protoflux_example_decrement.webp "File:Protoflux example decrement.webp")

How to use a simple decrement setup.


Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:Decrement&oldid=87519](https://wiki.resonite.com/index.php?title=ProtoFlux:Decrement&oldid=87519)"

Contents