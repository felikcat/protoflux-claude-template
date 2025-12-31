# ProtoFlux:Increment

> Source: https://wiki.resonite.com/ProtoFlux:Increment

\+ +

\*

OnWritten

OnFail

Variable

null

∅

Actions

Increments take Variable ( [Variable](https://wiki.resonite.com/Type:IVariable%602 "Type:IVariable`2") Pseudo-generic) as a global, and will increase the value that Variable ( [Variable](https://wiki.resonite.com/Type:IVariable%602 "Type:IVariable`2") Pseudo-generic) points to by 1.

![](https://wiki.resonite.com/images/d/dd/InformationIcon.svg)

Keep in mind this node will only work if given variables that can be incremented. Trying to increment a non numeric value like a [Boolean](https://wiki.resonite.com/Type:Bool "Type:Bool") or an [Enum](https://wiki.resonite.com/Category:Enums "Category:Enums") will not work.


Increments are a way to change a specified value without driving it. Instead you can use Increments to change a value in a similar fashion to changing the value through the inspector. Using Increments helps with performance too, since the values provided to the node only evaluate for one game tick while the node is being impulsed vs a driver which evaluates every game tick. This can also be used to reduce the amount of times code is evaluated. If you have to search the entire root for your code to find a slot and then do an operation, using Increments with your operations will help with performance since you're only searching once and not every single game tick.

When it comes to Increments, you can drag any matching [typed](https://wiki.resonite.com/Category:Type "Category:Type") source onto the Variable field to set that as the variable target. When you want to write to a [Local Variable Store](https://wiki.resonite.com/ProtoFlux:Local "ProtoFlux:Local"), [Data Model Variable Store](https://wiki.resonite.com/ProtoFlux:Data_Model_Store "ProtoFlux:Data Model Store"), or a [Store Variable Store](https://wiki.resonite.com/ProtoFlux:Store "ProtoFlux:Store"), you can grab the Variable field on Increments nodes and then choose the one you want in your context menu. This can save considerable time spent trying to find the type you want in another node menu.

![](https://wiki.resonite.com/images/c/c1/SuggestionIcon.svg)

If you just need to add + 1 to your [value](https://wiki.resonite.com/Value_Type "Value Type") using pure data, use the [Value Inc](https://wiki.resonite.com/ProtoFlux:Value_Inc "ProtoFlux:Value Inc") node instead.

If you need to add more than + 1 to your [value](https://wiki.resonite.com/Value_Type "Value Type"), use the [Add](https://wiki.resonite.com/ProtoFlux:Add "ProtoFlux:Add") node instead.

## Inputs

### \\* ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Call this to write the value.

## Outputs

### OnWritten ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

sends an impulse after \* ( [Call](https://wiki.resonite.com/Impulses "Impulses")) has been impulsed and the value pointed to by Variable ( [Variable](https://wiki.resonite.com/Type:IVariable%602 "Type:IVariable`2") Pseudo-generic) has been incremented.

### OnFail ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

sends an impulse after \* ( [Call](https://wiki.resonite.com/Impulses "Impulses")) has been impulsed and the value wasn't able to be incremented due to a missing target or Variable ( [Variable](https://wiki.resonite.com/Type:IVariable%602 "Type:IVariable`2") Pseudo-generic) not pointing to a valid [IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1").

## Globals

### Variable ( [Variable](https://wiki.resonite.com/Type:IVariable%602 "Type:IVariable`2") Pseudo-generic)

The numeric [Variable](https://wiki.resonite.com/Type:IVariable%602 "Type:IVariable`2") to increment by 1.

## Examples

- [How to use a simple increment setup.](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=Protoflux_example_increment.webp "File:Protoflux example increment.webp")

How to use a simple increment setup.


Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:Increment&oldid=87520](https://wiki.resonite.com/index.php?title=ProtoFlux:Increment&oldid=87520)"

Contents