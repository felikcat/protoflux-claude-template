# Component:CallbackRefArgument

> Source: https://wiki.resonite.com/Component:CallbackRefArgument

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:CallbackRefArgument&diff=97885) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/8/81/CallbackRefArgumentComponent.png/510px-CallbackRefArgumentComponent.png)](https://wiki.resonite.com/File:CallbackRefArgumentComponent.png) **Callback Ref Argument** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

Similar to [CallbackValueArgument](https://wiki.resonite.com/Component:CallbackValueArgument "Component:CallbackValueArgument") but instead of a value it's a reference for an action.

There are some [Sync Delegates](https://wiki.resonite.com/Sync_Delegate "Sync Delegate") in the game that match this component's requirements, but not many.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Reference` | **A** | The reference to give to `Callback` |
| `Callback` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") <A>** | The [Sync Delegate](https://wiki.resonite.com/Sync_Delegate "Sync Delegate") to call and provide `Reference` to. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `Call:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Call `Callback` sync delegate and provide it `Reference`. |
| `CallAndDestroy:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Do `Call()` and then destroy this component. |

Triggers
Collapse

## Usage

## Examples

Can be used to call a _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") <T>** (an action that takes a reference type) and give it `Reference` as an argument.

## Related Components

- [CallbackValueArgument](https://wiki.resonite.com/Component:CallbackValueArgument "Component:CallbackValueArgument")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:CallbackRefArgument&oldid=97885](https://wiki.resonite.com/index.php?title=Component:CallbackRefArgument&oldid=97885)"

Contents