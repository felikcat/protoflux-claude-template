# Component:CallbackValueArgument

> Source: https://wiki.resonite.com/Component:CallbackValueArgument

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/a/ae/CallbackValueArgument%601Component.png/510px-CallbackValueArgument%601Component.png)](https://wiki.resonite.com/File:CallbackValueArgument%601Component.png) **Callback Value Argument\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

_This article or section is a stub. You can help the Resonite wiki by expanding it._

This isn't very often used by the user, since there aren't many [Sync Delegates](https://wiki.resonite.com/Sync_Delegate "Sync Delegate") in the game that match this component's requirements.

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Value` | **A** | The value to give `Callback` when `Call()` or `CallAndDestroy()` is called. |
| `Callback` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") <A>** | The [Sync Delegate](https://wiki.resonite.com/Sync_Delegate "Sync Delegate") to call and send a value to. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `Call:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Call `Callback` sync delegate and provide it `Value`. |
| `CallAndDestroy:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Do `Call()` and then destroy this component. |

Triggers
Collapse

## Examples

Can be used to call a _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") <A>** (an action that takes a value type) and give it `Value` as an argument.
For example, using [Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3") as this component's callback type allows for calling [RandomObjectSpawner SpawnAtPoint()](https://wiki.resonite.com/Component:RandomObjectSpawner "Component:RandomObjectSpawner") and giving it `Value` as the position on where to spawn the random object.

## See Also

- [CallbackRefArgument](https://wiki.resonite.com/Component:CallbackRefArgument "Component:CallbackRefArgument")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:CallbackValueArgument&oldid=97886](https://wiki.resonite.com/index.php?title=Component:CallbackValueArgument&oldid=97886)"

Contents