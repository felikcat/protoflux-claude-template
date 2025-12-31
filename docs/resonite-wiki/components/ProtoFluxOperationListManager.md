# Component:ProtoFluxOperationListManager

> Source: https://wiki.resonite.com/Component:ProtoFluxOperationListManager

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/7/7b/ProtoFluxOperationListManagerComponent.png/510px-ProtoFluxOperationListManagerComponent.png)](https://wiki.resonite.com/File:ProtoFluxOperationListManagerComponent.png) **Proto Flux Operation List Manager** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ProtoFluxOperationListManager** component is used for the visuals in the [ProtoFlux:Sequence](https://wiki.resonite.com/ProtoFlux:Sequence "ProtoFlux:Sequence") and [ProtoFlux:Async Sequence](https://wiki.resonite.com/ProtoFlux:Async_Sequence "ProtoFlux:Async Sequence") nodes.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Visual` | **[ProtoFluxNodeVisual](https://wiki.resonite.com/Component:ProtoFluxNodeVisual "Component:ProtoFluxNodeVisual")** | The ProtoFlux visual this is a part of. |
| `List` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [ISyncList](https://wiki.resonite.com/Type:ISyncList "Type:ISyncList") >** | The list this is modifying. |
| `MinElements` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The minimum number of items allowed in the list. |
| `AddButtonEnabled` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | The enabled field of the add element list. |
| `RemoveButtonEnabled` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | The enabled field of the remove element list. |
| `_elements` | _[list](https://wiki.resonite.com/Type:SyncRefList%601 "Type:SyncRefList`1")_ of **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The list of UI elements being used to display the elements in `List` |
| `SupportsAsync` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the elements support Async input/output. |

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

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ProtoFluxOperationListManager&oldid=106521](https://wiki.resonite.com/index.php?title=Component:ProtoFluxOperationListManager&oldid=106521)"

Contents