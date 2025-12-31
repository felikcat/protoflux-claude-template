# ProtoFlux:ReferenceAsVariable

> Source: https://wiki.resonite.com/ProtoFlux:ReferenceAsVariable

Reference As Variable<T>

Reference

\*

Core

The **Reference As Variable** node transforms an [SyncRef](https://wiki.resonite.com/Type:SyncRef "Type:SyncRef") of the given type into an [IVariable](https://wiki.resonite.com/Type:IVariable "Type:IVariable") that can then be written to with an [Indirect Write](https://wiki.resonite.com/ProtoFlux:Indirect_Write "ProtoFlux:Indirect Write") node.

This node implements IVariable itself. This means that one may drag the output of this node into a normal [Write](https://wiki.resonite.com/ProtoFlux:Write "ProtoFlux:Write") node and write to the given SyncRef. This is actually more performant than using an Indirect Write, as a normal write node does not check if the variable changes every time it is pulsed. However, The performance gain diminishes the more often the input SyncRef changes, being roughly equal if the SyncRef changes at every write call.

## Inputs

### Reference ( [SyncRef<T>](https://wiki.resonite.com/Type:SyncRef%601 "Type:SyncRef`1"))

The SyncRef of type T to transform into a variable.

## Outputs

### \\* ( [Variable](https://wiki.resonite.com/Type:IVariable%602 "Type:IVariable`2"))

A variable created from the given `SyncRef`.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:ReferenceAsVariable&oldid=110573](https://wiki.resonite.com/index.php?title=ProtoFlux:ReferenceAsVariable&oldid=110573)"

Contents