# Component:ProtoFluxOperationProxy

> Source: https://wiki.resonite.com/Component:ProtoFluxOperationProxy

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/1/1b/ProtoFluxOperationProxyComponent.png/510px-ProtoFluxOperationProxyComponent.png)](https://wiki.resonite.com/File:ProtoFluxOperationProxyComponent.png) **Proto Flux Operation Proxy** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ProtoFluxOperationProxy** component is used to allow plugging impulse wires into protoflux visuals.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Node` | **[ProtoFluxNode](https://wiki.resonite.com/Type:ProtoFluxNode "Type:ProtoFluxNode")** | The protoflux node this is pointing to. |
| `ElementName` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The name of the input this is targeting. |
| `IsDynamic` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether or not this is dynamic. |
| `Index` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The index from top to bottom of the node's inputs. |
| `ConnectPoint` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The point the wire should connect to. |
| `NodeOperation` | **[INodeOperation](https://wiki.resonite.com/index.php?title=Type:INodeOperation&action=edit&redlink=1 "Type:INodeOperation (page does not exist)")** | The node operation target (impulse target) this is a connector for. |
| `IsAsync` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the impulse input type is async. |

Fields
Collapse

## Usage

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ProtoFluxOperationProxy&oldid=106524](https://wiki.resonite.com/index.php?title=Component:ProtoFluxOperationProxy&oldid=106524)"

Contents