# Component:ProtoFluxInputProxy

> Source: https://wiki.resonite.com/Component:ProtoFluxInputProxy

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/0/0d/ProtoFluxInputProxyComponent.png/510px-ProtoFluxInputProxyComponent.png)](https://wiki.resonite.com/File:ProtoFluxInputProxyComponent.png) **Proto Flux Input Proxy** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ProtoFluxInputProxy** component is used to manage the input sockets of protoflux nodes, making components become the actual visuals the user uses to interact with protoflux with. Otherwise, users would have to use purely the developer tool.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Node` | **[ProtoFluxNode](https://wiki.resonite.com/Type:ProtoFluxNode "Type:ProtoFluxNode")** | The ProtoFlux component whose input you wish to proxy. |
| `ElementName` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The name that appears when you hover this input with a Flux Tool. |
| `IsDynamic` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this input can be converted by inputting a different type. |
| `Index` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The index in a list if this points to a list of inputs/outputs. |
| `ConnectPoint` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | What Slot a wire visual parents itself under. |
| `Wire` | _direct_ **[CleanupRef\`1](https://wiki.resonite.com/Type:CleanupRef%601 "Type:CleanupRef`1") < [ProtoFluxWireManager](https://wiki.resonite.com/Component:ProtoFluxWireManager "Component:ProtoFluxWireManager") >** | The wire Manager handling the visual for the connection to this connector. |
| `NodeInput` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [ISyncRef](https://wiki.resonite.com/Type:ISyncRef "Type:ISyncRef") >** | The field on a protoflux node Component this connector is being used as a way to connect to. |
| `InputType` | _direct_ **[SyncType](https://wiki.resonite.com/Type:SyncType "Type:SyncType")** | The type of the input this proxy is for. |

Fields
Collapse

## Usage

Used to manage the wire visuals and interfacing with protoflux Components and their visuals.

## Examples

## See Also

- [ProtoFlux](https://wiki.resonite.com/ProtoFlux "ProtoFlux")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ProtoFluxInputProxy&oldid=106432](https://wiki.resonite.com/index.php?title=Component:ProtoFluxInputProxy&oldid=106432)"

Contents