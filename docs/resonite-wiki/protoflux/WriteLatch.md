# ProtoFlux:WriteLatch

> Source: https://wiki.resonite.com/ProtoFlux:WriteLatch

Write Latch

Set

OnSet

Reset

OnReset

SetValue

OnFail

ResetValue

Variable

null

∅

Actions

Write latches take a Variable ( [Variable](https://wiki.resonite.com/Type:IVariable%602 "Type:IVariable`2")) as a global input, and the Variable will determine what SetValue (Generic) and ResetValue (Generic) will take as a value. The set and reset value inputs will never take different types from each other.

Write Latches are a way to change a specified value without driving it. Instead you can use Write Latches to change a value in a similar fashion to changing the value through the inspector. Using Write Latches helps with performance too, since the values provided to the node only evaluate for one game tick while the node is being impulsed vs a driver which evaluates every game tick. This can also be used to reduce the amount of times code is evaluated. If you have to search the entire root for your code to find a slot and then do an operation, using Write Latches with your operations will help with performance since you're only searching once and not every single game tick.

When it comes to Write Latches, you can drag any matching [typed](https://wiki.resonite.com/Category:Type "Category:Type") source onto the Variable field to set that as the variable target. When you want to write to a [Local Variable Store](https://wiki.resonite.com/ProtoFlux:Local "ProtoFlux:Local"), [Data Model Variable Store](https://wiki.resonite.com/ProtoFlux:Data_Model_Store "ProtoFlux:Data Model Store"), or a [Store Variable Store](https://wiki.resonite.com/ProtoFlux:Store "ProtoFlux:Store"), you can grab the Variable field on Write Latches nodes and then choose the one you want in your context menu. This can save considerable time spent trying to find the type you want in another node menu.

## Inputs

### Reset ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Call this to set the value pointed to by Variable ( [Variable](https://wiki.resonite.com/Type:IVariable%602 "Type:IVariable`2") Generic) to the ResetValue (Generic) input.

### Set ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Call this to set the value pointed to by Variable ( [Variable](https://wiki.resonite.com/Type:IVariable%602 "Type:IVariable`2") Generic) to the SetValue (Generic) input.

### SetValue (Generic)

[Value](https://wiki.resonite.com/Category:Type "Category:Type") to write to the value pointed to by Variable ( [Variable](https://wiki.resonite.com/Type:IVariable%602 "Type:IVariable`2") Generic) upon calling Set ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

### ResetValue (Generic)

[Value](https://wiki.resonite.com/Category:Type "Category:Type") to write to the value pointed to by Variable ( [Variable](https://wiki.resonite.com/Type:IVariable%602 "Type:IVariable`2") Generic) upon calling Reset ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

## Outputs

### OnSet ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

sends an impulse after SetValue ( [Call](https://wiki.resonite.com/Impulses "Impulses")) has been impulsed and the value pointed to by Variable ( [Variable](https://wiki.resonite.com/Type:IVariable%602 "Type:IVariable`2") Generic) has been set to SetValue (Generic).

### OnReset ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

sends an impulse after ResetValue ( [Call](https://wiki.resonite.com/Impulses "Impulses")) has been impulsed and the value pointed to by Variable ( [Variable](https://wiki.resonite.com/Type:IVariable%602 "Type:IVariable`2") Generic) has been set to ResetValue (Generic).

### OnFail (Continuation)

sends an impulse after either ResetValue ( [Call](https://wiki.resonite.com/Impulses "Impulses")) or SetValue ( [Call](https://wiki.resonite.com/Impulses "Impulses")) has been impulsed and the value wasn't able to be written due to a missing Variable ( [Variable](https://wiki.resonite.com/Type:IVariable%602 "Type:IVariable`2") Generic) Value.

## Globals

### Variable ( [Variable](https://wiki.resonite.com/Type:IVariable%602 "Type:IVariable`2") Generic)

The value source/ref source to write to.

## Examples

- [Example of a write latch node set up to write text to a data model store variable, set will set the text to "hello" and reset sets it back to "goodbye".](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=Protoflux_example_write_latch.webp "File:Protoflux example write latch.webp")

Example of a write latch node set up to write text to a data model store variable, set will set the text to "hello" and reset sets it back to "goodbye".


Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:WriteLatch&oldid=111169](https://wiki.resonite.com/index.php?title=ProtoFlux:WriteLatch&oldid=111169)"

Contents