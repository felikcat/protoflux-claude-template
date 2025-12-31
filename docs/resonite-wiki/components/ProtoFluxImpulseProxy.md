# Component:ProtoFluxImpulseProxy

> Source: https://wiki.resonite.com/Component:ProtoFluxImpulseProxy

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/f/ff/ProtoFluxImpulseProxyComponent.png/510px-ProtoFluxImpulseProxyComponent.png)](https://wiki.resonite.com/File:ProtoFluxImpulseProxyComponent.png) **Proto Flux Impulse Proxy** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ProtoFluxImpulseProxy** component interacts with the [ProtoFlux](https://wiki.resonite.com/ProtoFlux "ProtoFlux") tool and ProtoFlux in general to act as the relay for attaching impulses to ProtoFlux nodes.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Node` | **[ProtoFluxNode](https://wiki.resonite.com/Type:ProtoFluxNode "Type:ProtoFluxNode")** | The node this is proxying an impulse for |
| `ElementName` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The name of the element that this is attaching an impulse to. |
| `IsDynamic` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the impulse is dynamic |
| `Index` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The index of the property to make an impulse for. |
| `ConnectPoint` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | the slot to attach the wire end being connected. |
| `Wire` | _direct_ **[CleanupRef\`1](https://wiki.resonite.com/Type:CleanupRef%601 "Type:CleanupRef`1") < [ProtoFluxWireManager](https://wiki.resonite.com/Component:ProtoFluxWireManager "Component:ProtoFluxWireManager") >** | The wire being attached to this impulse proxy |
| `NodeImpulse` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [ISyncRef](https://wiki.resonite.com/Type:ISyncRef "Type:ISyncRef") >** | The impulse value field to target. |
| `ImpulseType` | **[ImpulseType](https://wiki.resonite.com/index.php?title=Type:ImpulseType&action=edit&redlink=1 "Type:ImpulseType (page does not exist)")** | the type of impulse this is for. |

Fields
Collapse

## Usage

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ProtoFluxImpulseProxy&oldid=106512](https://wiki.resonite.com/index.php?title=Component:ProtoFluxImpulseProxy&oldid=106512)"

Contents