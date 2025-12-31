# Component:ProtoFluxOutputListManager

> Source: https://wiki.resonite.com/Component:ProtoFluxOutputListManager

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/8/87/ProtoFluxOutputListManagerComponent.png/510px-ProtoFluxOutputListManagerComponent.png)](https://wiki.resonite.com/File:ProtoFluxOutputListManagerComponent.png) **Proto Flux Output List Manager** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ProtoFluxOutputListManager** component is used to manage a list of outputs on a ProtoFlux visual.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Visual` | **[ProtoFluxNodeVisual](https://wiki.resonite.com/Component:ProtoFluxNodeVisual "Component:ProtoFluxNodeVisual")** | The ProtoFlux visual this is a part of. |
| `List` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [ISyncList](https://wiki.resonite.com/Type:ISyncList "Type:ISyncList") >** | The list this is a visual for. |
| `MinElements` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The minimum elements allowed for the list. |
| `AddButtonEnabled` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | The enabled field of the add elements button. |
| `RemoveButtonEnabled` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | The enabled field of the remove elements button. |
| `_elements` | _[list](https://wiki.resonite.com/Type:SyncRefList%601 "Type:SyncRefList`1")_ of **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | A list of slots representing the UIX elements of the list of outputs. |
| `OutputType` | _direct_ **[SyncType](https://wiki.resonite.com/Type:SyncType "Type:SyncType")** | The C# Type of the list of outputs for the list this is managing. |

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

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ProtoFluxOutputListManager&oldid=106525](https://wiki.resonite.com/index.php?title=Component:ProtoFluxOutputListManager&oldid=106525)"

Contents