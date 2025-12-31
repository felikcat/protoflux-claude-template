# ProtoFlux:WriteToGlobal

> Source: https://wiki.resonite.com/ProtoFlux:WriteToGlobal

Write Global

\*

OnWritten

Value

OnFail

Global

null

∅

Core

The **Write To Global** node takes in a [value](https://wiki.resonite.com/Value_type "Value type") or [reference](https://wiki.resonite.com/Reference_type "Reference type") and a [Global Value](https://wiki.resonite.com/Component:GlobalValue "Component:GlobalValue") component. When called, this node will write to the global value, which then can be used by any [Global To Output](https://wiki.resonite.com/ProtoFlux:Global_To_Output "ProtoFlux:Global To Output") node that has that component reference.

## Inputs

### \\* ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Calls an impulse to write to a global value component.

### Value (Generic)

The value to write into the global value component.

## Outputs

### OnWritten ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Fires when the value was successfully written.

### OnFail ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Fires when this node fails to write.

## Globals

### Global (Generic)

The global value component that is referenced.

## Examples

To make this work, you need the following things:

- [Write To Global](https://wiki.resonite.com/ProtoFlux:Write_To_Global "ProtoFlux:Write To Global")
- [Global To Output](https://wiki.resonite.com/ProtoFlux:Global_To_Output "ProtoFlux:Global To Output")
- [Global Value](https://wiki.resonite.com/Component:GlobalValue "Component:GlobalValue") or [Global Reference](https://wiki.resonite.com/Component:GlobalReference "Component:GlobalReference")

Using primary on either global areas of the nodes will automatically make a GlobalValue/GlobalReference component. These can be accessed currently through the inspector only. Once opened in the inspector, if there are any GlobalToOutput nodes that automatically made GlobalValue/GlobalReference components on them, those can be removed in favor of any components made prior (either on WriteToGlobal nodes or on other slots that has those components)

The last step is to reference GlobalValue/GlobalReference component in the WriteToGlobal node (or from some other slot) to the field in the GlobalToOutput node. Then call the write node and notice the value change.

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

Keep in mind that the GlobalToOutput node will not update automatically if you have a display out from it already, using the [Continuously Changing Relay](https://wiki.resonite.com/ProtoFlux:Continuously_Changing_Relay "ProtoFlux:Continuously Changing Relay") will update these displays as you write values to see those displays update, although not recommended.


- [![ProtoFlux Global Example.](https://wiki.resonite.com/images/thumb/f/f8/ProtoFluxGlobalExample.png/480px-ProtoFluxGlobalExample.png)](https://wiki.resonite.com/File:ProtoFluxGlobalExample.png "ProtoFlux Global Example.")

ProtoFlux Global Example.


Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:WriteToGlobal&oldid=111175](https://wiki.resonite.com/index.php?title=ProtoFlux:WriteToGlobal&oldid=111175)"

Contents