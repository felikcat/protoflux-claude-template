# ProtoFlux:Write

> Source: https://wiki.resonite.com/ProtoFlux:Write

Write

\*

OnWritten

Value

OnFail

Variable

null

∅

Actions

Writes take Variable ( [Variable](https://wiki.resonite.com/Type:IVariable%602 "Type:IVariable`2")) as an input, and the type that Variable wraps will determine what Value (Generic) will take as a value. The node will then write Value (Generic) to the field Variable ( [Variable](https://wiki.resonite.com/Type:IVariable%602 "Type:IVariable`2")) wraps.

When it comes to Writes, you can drag any matching [typed](https://wiki.resonite.com/Category:Type "Category:Type") source onto the Variable field to set that as the variable target. When you want to write to a [Local Variable Store](https://wiki.resonite.com/ProtoFlux:Local "ProtoFlux:Local"), [Data Model Variable Store](https://wiki.resonite.com/ProtoFlux:Data_Model_Store "ProtoFlux:Data Model Store"), or a [Store Variable Store](https://wiki.resonite.com/ProtoFlux:Store "ProtoFlux:Store"), you can grab the Variable field on Writes nodes and then choose the one you want in your context menu. This can save considerable time spent trying to find the type you want in another node menu.

Writes are a way to change a specified value without driving it. Instead you can use Writes to change a value in a similar fashion to changing the value through the inspector. Using Writes helps with performance too, since the values provided to the node only evaluate for one game tick while the node is being impulsed vs a driver which evaluates every game tick. This can also be used to reduce the amount of times code is evaluated. If you have to search the entire root for your code to find a slot and then do an operation, using Writes with your operations will help with performance since you're only searching once and not every single game tick.

## Optimizations

The Write node can also be used to write to a Protoflux Source node instead of writing to a variable that is connected to a Drive node, enabling programs be be written with one less supporting node per Write node

## Inputs

### \\* ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Call this to write the value.

### Value (Generic)

[Value](https://wiki.resonite.com/Category:Type "Category:Type") to write to the value pointed to by Variable ( [Variable](https://wiki.resonite.com/Type:IVariable%602 "Type:IVariable`2"))

## Outputs

### OnWritten ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

sends an impulse after \* ( [Call](https://wiki.resonite.com/Impulses "Impulses")) has been impulsed and the value has been written.

### OnFail ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

sends an impulse after \* ( [Call](https://wiki.resonite.com/Impulses "Impulses")) has been impulsed and the value wasn't able to be written due to a missing target or a missing Variable ( [Variable](https://wiki.resonite.com/Type:IVariable%602 "Type:IVariable`2")) value

## Globals

### Variable ( [Variable](https://wiki.resonite.com/Type:IVariable%602 "Type:IVariable`2") Generic)

The [Variable](https://wiki.resonite.com/Type:IVariable%602 "Type:IVariable`2") to write to.

## Examples

- [![Example showing how to connect a source value to a write node by dragging a ribbon to the variable](https://wiki.resonite.com/images/thumb/d/d4/WriteNode_ConnectASourceToVariable.png/480px-WriteNode_ConnectASourceToVariable.png)](https://wiki.resonite.com/File:WriteNode_ConnectASourceToVariable.png "Example showing how to connect a source value to a write node by dragging a ribbon to the variable")

Example showing how to connect a source value to a write node by dragging a ribbon to the variable


Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:Write&oldid=112796](https://wiki.resonite.com/index.php?title=ProtoFlux:Write&oldid=112796)"

Contents