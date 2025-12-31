# Component:ButtonActionTrigger

> Source: https://wiki.resonite.com/Component:ButtonActionTrigger

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:ButtonActionTrigger&diff=90344) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/6/63/ButtonActionTriggerComponent.png/510px-ButtonActionTriggerComponent.png)](https://wiki.resonite.com/File:ButtonActionTriggerComponent.png) **ButtonActionTrigger** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ButtonActionTrigger** component is used for triggering C# [actions](https://wiki.resonite.com/Type:Action "Type:Action") (not to be confused with [impulses](https://wiki.resonite.com/Impulses "Impulses")) using the Interface [IButton](https://wiki.resonite.com/Type:IButton "Type:IButton"), such as [UIX Buttons](https://wiki.resonite.com/Button_(Component) "Button (Component)") or [Legacy Buttons](https://wiki.resonite.com/LegacyButton_(Component) "LegacyButton (Component)").

This component must be on the same [slot](https://wiki.resonite.com/Slot "Slot") as the [button](https://wiki.resonite.com/Type:IButton "Type:IButton") in order to be bound to it.

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `OnPressed` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | Triggered when the button is pressed |
| `OnPressing` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | Triggered when the button is pressed, before the `OnPressed` event |
| `OnReleased` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | Triggered when the button is released |

Fields
Collapse

## Usage

This component allows you to trigger [actions](https://wiki.resonite.com/Type:Action "Type:Action") on some special components, such as the [Random Object Spawner component](https://wiki.resonite.com/RandomObjectSpawner_(Component) "RandomObjectSpawner (Component)"), by dragging the reference to the target action into a trigger slot (such as `OnPressed`).

## Examples

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ButtonActionTrigger&oldid=90344](https://wiki.resonite.com/index.php?title=Component:ButtonActionTrigger&oldid=90344)"

Contents