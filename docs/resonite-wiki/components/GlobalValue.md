# Component:GlobalValue

> Source: https://wiki.resonite.com/Component:GlobalValue

Collapse **Component image**

[File:GlobalValue\`1Component.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=GlobalValue%601Component.png "File:GlobalValue`1Component.png") **GlobalValue<T>** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **GlobalValue<T>** component is used by [ProtoFlux](https://wiki.resonite.com/ProtoFlux "ProtoFlux") to define a [global](https://wiki.resonite.com/index.php?title=Global&action=edit&redlink=1 "Global (page does not exist)") of a [FrooxEngine value type](https://wiki.resonite.com/Value_type#In_FrooxEngine "Value type").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Value` | **T** | The underlying value of the global. |

Fields
Collapse

## Usage

When not using ProtoFlux, this component has no use over more idiomatic components such as a [ValueField](https://wiki.resonite.com/Component:ValueField "Component:ValueField").

When using ProtoFlux, the underlying value can be changed and any node that accepts a global input that references the component will update during execution. This can allow one to dynamically change things like [dynamic impulse receiver](https://wiki.resonite.com/ProtoFlux:Dynamic_Impulse_Receiver "ProtoFlux:Dynamic Impulse Receiver") tags.

This component can also simply be used for static global values that need to be referenced in a lot of places for when the overhead of [dynamic variables](https://wiki.resonite.com/Dynamic_variables "Dynamic variables") is undesirable. When combined with the [Global To Output](https://wiki.resonite.com/ProtoFlux:Global_To_Output "ProtoFlux:Global To Output") node, this component also provides more UX than sourcing a ValueField by being able to see the underlying value directly.

## See Also

- [Component:GlobalReference](https://wiki.resonite.com/Component:GlobalReference "Component:GlobalReference") for global [reference types](https://wiki.resonite.com/Reference_types "Reference types").
- [Component:GlobalDelegate](https://wiki.resonite.com/Component:GlobalDelegate "Component:GlobalDelegate") for global [sync delegates](https://wiki.resonite.com/index.php?title=Type:SyncDelegate&action=edit&redlink=1 "Type:SyncDelegate (page does not exist)").
- [ProtoFlux:Global To Output](https://wiki.resonite.com/ProtoFlux:Global_To_Output "ProtoFlux:Global To Output")
- [ProtoFlux:Write To Global](https://wiki.resonite.com/ProtoFlux:Write_To_Global "ProtoFlux:Write To Global")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:GlobalValue&oldid=99322](https://wiki.resonite.com/index.php?title=Component:GlobalValue&oldid=99322)"

Contents