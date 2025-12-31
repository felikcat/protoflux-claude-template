# ProtoFlux:ReferenceToOutput

> Source: https://wiki.resonite.com/ProtoFlux:ReferenceToOutput

Ref To Output

\*

Reference

null

∅

Core

The **Reference To Output** node takes a [Global](https://wiki.resonite.com/index.php?title=Global&action=edit&redlink=1 "Global (page does not exist)") ProtoFlux reference and returns the [IVariable](https://wiki.resonite.com/Type:IVariable%602 "Type:IVariable`2") that can be used for an [Indirect Write](https://wiki.resonite.com/ProtoFlux:Indirect_Write "ProtoFlux:Indirect Write").

This node is automatically created when attaching an applicable node output ( [Data Model Store](https://wiki.resonite.com/ProtoFlux:Data_Model_Store "ProtoFlux:Data Model Store"), [Store](https://wiki.resonite.com/ProtoFlux:Store "ProtoFlux:Store"), [Local](https://wiki.resonite.com/ProtoFlux:Local "ProtoFlux:Local"), or [Source](https://wiki.resonite.com/ProtoFlux:Source "ProtoFlux:Source")) into an input that requires an IVariable. To create this node from the node menu, one must use the assembly type names for IVariable and [ExecutionContent](https://wiki.resonite.com/index.php?title=Type:ExecutionContent&action=edit&redlink=1 "Type:ExecutionContent (page does not exist)"). An example valid type for this node is `ProtoFlux.Runtimes.Execution.IVariable<ProtoFlux.Runtimes.Execution.ExecutionContext,string>`.

## Outputs

### \\* ( [IVariable](https://wiki.resonite.com/Type:IVariable%602 "Type:IVariable`2"))

The IVariable wrapper of `Reference`.

## Globals

### Reference ( [IVariable](https://wiki.resonite.com/Type:IVariable%602 "Type:IVariable`2"))

The `IProtoFluxNode<IVariable<C,T>>` to output. Common cases for this are a [Data Model Store](https://wiki.resonite.com/ProtoFlux:Data_Model_Store "ProtoFlux:Data Model Store"), [Store](https://wiki.resonite.com/ProtoFlux:Store "ProtoFlux:Store"), [Local](https://wiki.resonite.com/ProtoFlux:Local "ProtoFlux:Local"), or [Source](https://wiki.resonite.com/ProtoFlux:Source "ProtoFlux:Source").

## Examples

- [![A simple example or writing to a source.](https://wiki.resonite.com/images/thumb/d/d0/RefToOutputExample01.png/480px-RefToOutputExample01.png)](https://wiki.resonite.com/File:RefToOutputExample01.png "A simple example or writing to a source.")

A simple example or writing to a source.

- [![Different ways of writing to the Value of a Component:ValueField.](https://wiki.resonite.com/images/thumb/8/80/ProtoFlux_Example_Different_Ways_of_Writes.webp/480px-ProtoFlux_Example_Different_Ways_of_Writes.webp.png)](https://wiki.resonite.com/File:ProtoFlux_Example_Different_Ways_of_Writes.webp "Different ways of writing to the Value of a Component:ValueField.")

Different ways of writing to the `Value` of a [Component:ValueField](https://wiki.resonite.com/Component:ValueField "Component:ValueField").


## See Also

- [ProtoFlux:Field As Variable](https://wiki.resonite.com/ProtoFlux:Field_As_Variable "ProtoFlux:Field As Variable"), an easier way to achieve this behavior if one is working with [IFields](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") and not stores.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:ReferenceToOutput&oldid=110583](https://wiki.resonite.com/index.php?title=ProtoFlux:ReferenceToOutput&oldid=110583)"

Contents