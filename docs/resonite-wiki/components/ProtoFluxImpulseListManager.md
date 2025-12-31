# Component:ProtoFluxImpulseListManager

> Source: https://wiki.resonite.com/Component:ProtoFluxImpulseListManager

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/c/ce/ProtoFluxImpulseListManagerComponent.png/510px-ProtoFluxImpulseListManagerComponent.png)](https://wiki.resonite.com/File:ProtoFluxImpulseListManagerComponent.png) **Proto Flux Impulse List Manager** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ProtoFluxImpulseListManager** component is used to manage lists and their visuals like in the sequence ProtoFlux node.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Visual` | **[ProtoFluxNodeVisual](https://wiki.resonite.com/Component:ProtoFluxNodeVisual "Component:ProtoFluxNodeVisual")** | The visual of the protoflux node this is making a list for. |
| `List` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [ISyncList](https://wiki.resonite.com/Type:ISyncList "Type:ISyncList") >** | The list this is managing and making a UI for. |
| `MinElements` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The minimum elements allowed in the list. |
| `AddButtonEnabled` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | The enabled field of adding a list item. |
| `RemoveButtonEnabled` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | The enabled field of removing a list item. |
| `_elements` | _[list](https://wiki.resonite.com/Type:SyncRefList%601 "Type:SyncRefList`1")_ of **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The list of elements defining the impulse connectors. |
| `ImpulseType` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [ImpulseType](https://wiki.resonite.com/index.php?title=Type:ImpulseType&action=edit&redlink=1 "Type:ImpulseType (page does not exist)") >** | The type of impulse this is using (ex: Async or normal) |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `AddElement:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | X | Called when the add element button is touched. |
| `RemoveElement:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | X | Called when the remove element button is touched. |

Triggers
Collapse

## Usage

Used in nodes like the sequence and async sequence nodes.

## Examples

## See Also

- [ProtoFlux](https://wiki.resonite.com/ProtoFlux "ProtoFlux")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ProtoFluxImpulseListManager&oldid=106431](https://wiki.resonite.com/index.php?title=Component:ProtoFluxImpulseListManager&oldid=106431)"

Contents