# Component:ButtonValueActionTrigger

> Source: https://wiki.resonite.com/Component:ButtonValueActionTrigger

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/7/77/ButtonValueActionTrigger%601Component.png/510px-ButtonValueActionTrigger%601Component.png)](https://wiki.resonite.com/File:ButtonValueActionTrigger%601Component.png) **Button Value Action Trigger\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ButtonValueActionTrigger** component receives any [Button Event](https://wiki.resonite.com/Button_Event "Button Event") and uses it to trigger a [Sync Delegate](https://wiki.resonite.com/Sync_Delegate "Sync Delegate") and sends a value to it.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `OnPressed` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") <T>** | triggers while sending `Value` when this component receives a [Button Event](https://wiki.resonite.com/Button_Event "Button Event") of type OnPressed. |
| `OnPressing` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") <T>** | triggers while sending `Value` when this component receives a [Button Event](https://wiki.resonite.com/Button_Event "Button Event") of type OnPressing. |
| `OnReleased` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") <T>** | triggers while sending `Value` when this component receives a [Button Event](https://wiki.resonite.com/Button_Event "Button Event") of type OnReleased. |
| `Value` | **T** | The value to send to any `OnPressed`, `OnPressing`, and/or `OnReleased`. |

Fields
Collapse

## Usage

Attach to a slot with a button, or a slot targeted by a [Component:ButtonRelay](https://wiki.resonite.com/Component:ButtonRelay "Component:ButtonRelay") or related. Then, find a [Sync Delegate](https://wiki.resonite.com/Sync_Delegate "Sync Delegate") to trigger using this component. Lastly, put the sync delegate into any `OnPressed`, `OnPressing`, and/or `OnReleased`; then provide `Value`

## Examples

## See Also

- [Component:ButtonRelay](https://wiki.resonite.com/Component:ButtonRelay "Component:ButtonRelay")
- [Button Events](https://wiki.resonite.com/Button_Events "Button Events")
- [Sync Delegates](https://wiki.resonite.com/Sync_Delegates "Sync Delegates") <\- To learn what they are and how to find them.

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ButtonValueActionTrigger&oldid=92320](https://wiki.resonite.com/index.php?title=Component:ButtonValueActionTrigger&oldid=92320)"

Contents