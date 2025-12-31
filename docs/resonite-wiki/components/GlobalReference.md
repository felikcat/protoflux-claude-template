# Component:GlobalReference

> Source: https://wiki.resonite.com/Component:GlobalReference

Collapse **Component image**

[File:GlobalReference\`1Component.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=GlobalReference%601Component.png "File:GlobalReference`1Component.png") **Global Reference<T>** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **GlobalReference<T>** component is used by [ProtoFlux](https://wiki.resonite.com/ProtoFlux "ProtoFlux") to define a [global](https://wiki.resonite.com/index.php?title=Global&action=edit&redlink=1 "Global (page does not exist)") of a [reference type](https://wiki.resonite.com/Reference_type "Reference type").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Reference` | **T** | The underlying reference of the global. |

Fields
Collapse

## Usage

When not using ProtoFlux, This component has no use over more idiomatic components such as a [ReferenceField](https://wiki.resonite.com/Component:ReferenceField "Component:ReferenceField").

This node can be used with a global to output and a node that accepts it's Type as a global (ex: raw data tool tip events) this allows to use a global variable to be used in Flux as a value at the same time without needing to drive the global value in the node using it for its data.

When using ProtoFlux, the underlying reference can be changed and any node that accepts a global reference input that references the component will update during execution. This can allow one to dynamically change things like where [source](https://wiki.resonite.com/ProtoFlux:Source "ProtoFlux:Source") nodes point to.

This component can also simply be used for static global references that need to be referenced in a lot of places for when the overhead of [dynamic variables](https://wiki.resonite.com/Dynamic_variables "Dynamic variables") is undesirable. When combined with the [Global To Output](https://wiki.resonite.com/ProtoFlux:Global_To_Output "ProtoFlux:Global To Output") node, this component provides more UX than sourcing a ReferenceField by being able to see the underlying reference directly.

## See Also

- [Component:GlobalValue](https://wiki.resonite.com/Component:GlobalValue "Component:GlobalValue") for global [value types](https://wiki.resonite.com/Value_types "Value types").
- [Component:GlobalDelegate](https://wiki.resonite.com/Component:GlobalDelegate "Component:GlobalDelegate") for global [sync delegates](https://wiki.resonite.com/index.php?title=Type:SyncDelegate&action=edit&redlink=1 "Type:SyncDelegate (page does not exist)").
- [ProtoFlux:Global To Output](https://wiki.resonite.com/ProtoFlux:Global_To_Output "ProtoFlux:Global To Output")
- [ProtoFlux:Write To Global](https://wiki.resonite.com/ProtoFlux:Write_To_Global "ProtoFlux:Write To Global")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:GlobalReference&oldid=106429](https://wiki.resonite.com/index.php?title=Component:GlobalReference&oldid=106429)"

Contents