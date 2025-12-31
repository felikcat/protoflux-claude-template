# Component:ProtoFluxReferenceProxy

> Source: https://wiki.resonite.com/Component:ProtoFluxReferenceProxy

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/c/c4/ProtoFluxReferenceProxyComponent.png/510px-ProtoFluxReferenceProxyComponent.png)](https://wiki.resonite.com/File:ProtoFluxReferenceProxyComponent.png) **Proto Flux Reference Proxy** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ProtoFluxReferenceProxy** component is used to usually manage global references like on write node write targets and the monitoring slot on the slot events node.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Node` | **[ProtoFluxNode](https://wiki.resonite.com/Type:ProtoFluxNode "Type:ProtoFluxNode")** | The node this is making a visual for. |
| `ElementName` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The element this is pointing to. |
| `ValueType` | _direct_ **[SyncType](https://wiki.resonite.com/Type:SyncType "Type:SyncType")** | the type of the value input this is pointing to. |
| `_label` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | The text element of the element this is for. |
| `_proxyVisual` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | The button to set the input field value with. |
| `_refProxySource` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [ReferenceProxySource](https://wiki.resonite.com/Component:ReferenceProxySource "Component:ReferenceProxySource") >** | the component that handles grabbing the value of the field this points to via UIX. |
| `NodeReference` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [ISyncRef](https://wiki.resonite.com/Type:ISyncRef "Type:ISyncRef") >** | The node the value field points to, if it should point to a protoflux node like for a write node. |
| `Arrow` | _direct_ **[CleanupRef\`1](https://wiki.resonite.com/Type:CleanupRef%601 "Type:CleanupRef`1") < [ProtofluxArrowManager](https://wiki.resonite.com/Component:ProtofluxArrowManager "Component:ProtofluxArrowManager") >** | the arrow pointing to a protoflux node if the value field's value points to a protoflux node. |
| `ConnectPoint` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot that should act as the connector point. |
| `_currentName` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [IValue\`1](https://wiki.resonite.com/Type:IValue%601 "Type:IValue`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >>** | The field to drive with the current name of the value that this component's value field is pointing to. |
| `_selfHovering` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [IValue\`1](https://wiki.resonite.com/Type:IValue%601 "Type:IValue`1") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >>** | The field to drive with whether or not this element is being hovered over. |
| `_targetHovering` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [IValue\`1](https://wiki.resonite.com/Type:IValue%601 "Type:IValue`1") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >>** | The field to drive with whether or not the element this is targeting is a node and is being hovered over. |
| `_arrowManagerEnabled` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | The field to drive in order to enable/disable the arrow manager. |
| `_arrowRendererEnabled` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | The field to drive in order to enable/disable the arrow manager's arrow visual. |

Fields
Collapse

## Usage

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ProtoFluxReferenceProxy&oldid=106527](https://wiki.resonite.com/index.php?title=Component:ProtoFluxReferenceProxy&oldid=106527)"

Contents