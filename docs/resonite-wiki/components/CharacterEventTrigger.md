# Component:CharacterEventTrigger

> Source: https://wiki.resonite.com/Component:CharacterEventTrigger

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:CharacterEventTrigger&diff=91364) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/a/af/CharacterEventTriggerComponent.png/510px-CharacterEventTriggerComponent.png)](https://wiki.resonite.com/File:CharacterEventTriggerComponent.png) **CharacterEventTrigger** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **CharacterEventTrigger** component invokes [Action<Float3>](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") triggers whenever a user enters or exits an attached collider.

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `TriggersOnly` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to only use Trigger type colliders on this hierarchy when detecting character collisions. |
| `TriggerEntered` | _[list](https://wiki.resonite.com/Type:SyncDelegateList%601 "Type:SyncDelegateList`1")_ of **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") < [Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3") >** | Triggered when a user enters a collider attached to the parent slot |
| `TriggerLeft` | _[list](https://wiki.resonite.com/Type:SyncDelegateList%601 "Type:SyncDelegateList`1")_ of **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") < [Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3") >** | Triggered when a user exits a collider attached to the parent slot |
| `IgnoreParentUser` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | If this component is under a user in the hierarchy, events from that user are ignored. |

Fields
Collapse

## Behavior

## Examples

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:CharacterEventTrigger&oldid=91364](https://wiki.resonite.com/index.php?title=Component:CharacterEventTrigger&oldid=91364)"

Contents