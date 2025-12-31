# ProtoFlux:Source

> Source: https://wiki.resonite.com/ProtoFlux:Source

_HTML Visual unavailable due to wiki limitations_

[![Six source nodes of type string, string, bool, float3, floatQ, and int all outputting to display nodes.](https://wiki.resonite.com/images/thumb/7/79/ProtoFlux_Visuals_Source_Display.webp/300px-ProtoFlux_Visuals_Source_Display.webp.png)](https://wiki.resonite.com/File:ProtoFlux_Visuals_Source_Display.webp) Source nodes for the base fields of an empty slot being outputted to display nodes.

The **Source** node allows one to access the value of the primitive or object that an [IValue<T>](https://wiki.resonite.com/Type:IValue%601 "Type:IValue`1") contains. This node almost never should be created directly through the node menu, lest one knows exactly what they are doing. Source nodes are created by dragging out a field from an inspector, opening the [Context menu](https://wiki.resonite.com/Context_menu "Context menu"), then pressing `Source`.

To access the underlying value that any arbitrary IValue<T> contains, one can spawn out a bare version of this node from the ProtoFlux menu, attach a [GlobalReference<IValue<T>>](https://wiki.resonite.com/Component:GlobalReference "Component:GlobalReference") to the slot of the node, drag the component header into the `Source` field of the Source node, and finally input the IValue<T> into the <source>Reference field of the GlobalReference. This can allow for a more efficient way to conditionally change values if said values are in different fields.

## See Also

- [ProtoFlux:ReferenceSource](https://wiki.resonite.com/ProtoFlux:ReferenceSource "ProtoFlux:ReferenceSource")
- [ProtoFlux:ChangeableSource](https://wiki.resonite.com/index.php?title=ProtoFlux:ChangeableSource&action=edit&redlink=1 "ProtoFlux:ChangeableSource (page does not exist)")

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:Source&oldid=100151](https://wiki.resonite.com/index.php?title=ProtoFlux:Source&oldid=100151)"

Contents