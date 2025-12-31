# Component:ProtoFluxGlobalRefProxy

> Source: https://wiki.resonite.com/Component:ProtoFluxGlobalRefProxy

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/6/64/ProtoFluxGlobalRefProxyComponent.png/510px-ProtoFluxGlobalRefProxyComponent.png)](https://wiki.resonite.com/File:ProtoFluxGlobalRefProxyComponent.png) **Proto Flux Global Ref Proxy** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ProtoFluxGlobalRefProxy** component allows for a piece of UI to act as a relay for interacting with global value component.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Node` | **[ProtoFluxNode](https://wiki.resonite.com/Type:ProtoFluxNode "Type:ProtoFluxNode")** | The node that this is on. |
| `ElementName` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | the name of the target component. |
| `ValueType` | _direct_ **[SyncType](https://wiki.resonite.com/Type:SyncType "Type:SyncType")** | The type of the value being held. |
| `_label` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | The field to drive with global value properties to make a name. |
| `_proxyVisual` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | The Button used for the proxy surrounding visual. |
| `_refProxySource` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [ReferenceProxySource](https://wiki.resonite.com/Component:ReferenceProxySource "Component:ReferenceProxySource") >** | The proxy used to get the global ref. |
| `TargetGlobalRef` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [ISyncRef](https://wiki.resonite.com/Type:ISyncRef "Type:ISyncRef") >** | The target global reference this visual has been made for. |
| `_currentProxy` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [IGlobalValueProxy](https://wiki.resonite.com/index.php?title=Type:IGlobalValueProxy&action=edit&redlink=1 "Type:IGlobalValueProxy (page does not exist)") >** | The current proxy this is using. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `OnProxyButtonPressed:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the proxy button is touched on the visual. |

Triggers
Collapse

## Usage

Used in nodes like raw data tool events to show the field for the raw data tool. This is also used to interact with said visual.

## Examples

## See Also

- [ProtoFlux](https://wiki.resonite.com/ProtoFlux "ProtoFlux")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ProtoFluxGlobalRefProxy&oldid=106430](https://wiki.resonite.com/index.php?title=Component:ProtoFluxGlobalRefProxy&oldid=106430)"

Contents