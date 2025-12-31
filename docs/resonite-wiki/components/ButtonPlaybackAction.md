# Component:ButtonPlaybackAction

> Source: https://wiki.resonite.com/Component:ButtonPlaybackAction

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:ButtonPlaybackAction&diff=90373) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/d/da/ButtonPlaybackActionComponent.png/510px-ButtonPlaybackActionComponent.png)](https://wiki.resonite.com/File:ButtonPlaybackActionComponent.png) **Button Playback Action** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ButtonPlaybackAction** component takes in an [IPlayable](https://wiki.resonite.com/Type:IPlayable "Type:IPlayable"). When an [IButton](https://wiki.resonite.com/Type:IButton "Type:IButton") is pressed while this component is in the same [slot](https://wiki.resonite.com/Slot "Slot"), it will set the action on this playable media depending on what is set up in this component.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Playback` | **[IPlayable](https://wiki.resonite.com/Type:IPlayable "Type:IPlayable")** | The playable media itself. |
| `OnHover` | **[PlaybackAction](https://wiki.resonite.com/Type:PlaybackAction "Type:PlaybackAction")** | The action to take when the button is hovered over. |
| `OnLeave` | **[PlaybackAction](https://wiki.resonite.com/Type:PlaybackAction "Type:PlaybackAction")** | The action to take when the button is left. |
| `OnPress` | **[PlaybackAction](https://wiki.resonite.com/Type:PlaybackAction "Type:PlaybackAction")** | The action to take when the button is pressed. |
| `OnRelease` | **[PlaybackAction](https://wiki.resonite.com/Type:PlaybackAction "Type:PlaybackAction")** | The action to take when the button is released. |

Fields
Collapse

## Usage

Basically your media buttons (`Play`, `Pause`, `Resume`, and `Stop`) that can be setup anywhere.

## Examples

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ButtonPlaybackAction&oldid=90373](https://wiki.resonite.com/index.php?title=Component:ButtonPlaybackAction&oldid=90373)"

Contents