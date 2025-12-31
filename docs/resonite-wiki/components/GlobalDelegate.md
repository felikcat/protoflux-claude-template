# Component:GlobalDelegate

> Source: https://wiki.resonite.com/Component:GlobalDelegate

Collapse **Component image**

[File:GlobalDelegate\`1Component.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=GlobalDelegate%601Component.png "File:GlobalDelegate`1Component.png") **GlobalDelegate<T>** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **GlobalDelegate<T>** component is used by [ProtoFlux](https://wiki.resonite.com/ProtoFlux "ProtoFlux") to define a [global](https://wiki.resonite.com/index.php?title=Global&action=edit&redlink=1 "Global (page does not exist)") of a [sync delegate](https://wiki.resonite.com/index.php?title=Type:SyncDelegate&action=edit&redlink=1 "Type:SyncDelegate (page does not exist)") type.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Delegate` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **T** | The underlying delegate of the global. |

Fields
Collapse

## Usage

When not using ProtoFlux, This component has no use over more idiomatic components such as a [ReferenceField<SyncField<WorldDelegate>>](https://wiki.resonite.com/Component:ReferenceField "Component:ReferenceField").

When using ProtoFlux, the underlying reference can be changed and any node that accepts a global reference input that references the component will update during execution. This can allow one to dynamically change things like where [method proxy](https://wiki.resonite.com/ProtoFlux:Method_Proxy "ProtoFlux:Method Proxy") nodes point to.

This component can also simply be used for static global delegates that need to be referenced in a lot of places for when the overhead of [dynamic variables](https://wiki.resonite.com/Dynamic_variables "Dynamic variables") is undesirable. When combined with the [Global To Output](https://wiki.resonite.com/ProtoFlux:Global_To_Output "ProtoFlux:Global To Output") node, this component provides more UX than sourcing a ReferenceField<SyncField<WorldDelegate>> by being able to see the underlying delegate directly from the UI.

## Examples

## See Also

- [Component:GlobalValue](https://wiki.resonite.com/Component:GlobalValue "Component:GlobalValue") for global [value types](https://wiki.resonite.com/Value_types "Value types").
- [Component:GlobalReference](https://wiki.resonite.com/Component:GlobalReference "Component:GlobalReference") for global [reference types](https://wiki.resonite.com/Reference_types "Reference types").
- [ProtoFlux:Global To Output](https://wiki.resonite.com/ProtoFlux:Global_To_Output "ProtoFlux:Global To Output")
- [ProtoFlux:Write To Global](https://wiki.resonite.com/ProtoFlux:Write_To_Global "ProtoFlux:Write To Global")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:GlobalDelegate&oldid=99324](https://wiki.resonite.com/index.php?title=Component:GlobalDelegate&oldid=99324)"

Contents