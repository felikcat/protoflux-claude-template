# Component:TouchWorldLink

> Source: https://wiki.resonite.com/Component:TouchWorldLink

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:TouchWorldLink&diff=95767) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/4/40/TouchWorldLinkComponent.png/510px-TouchWorldLinkComponent.png)](https://wiki.resonite.com/File:TouchWorldLinkComponent.png) **Touch World Link** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **TouchWorldLink** component when touched allows a user to go to the world of the given link.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `AcceptPhysicalTouch` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to allow [Component:TipTouchSources](https://wiki.resonite.com/Component:TipTouchSource "Component:TipTouchSource") to interact with/activate this component. |
| `AcceptRemoteTouch` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this component allows interaction via the user's interaction laser. |
| `AcceptOutOfSightTouch` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether or not to allow interaction with this component if it is out of the user's view. |
| `Vibrate` | **[VibratePreset](https://wiki.resonite.com/Type:VibratePreset "Type:VibratePreset")** | How to vibrate the haptics of the hand that touched this component. |
| `LastOpened` | _direct_ **[SyncTime](https://wiki.resonite.com/Type:SyncTime "Type:SyncTime")** | The last world time this component was pressed. |
| `WorldLink` | **[WorldLink](https://wiki.resonite.com/Component:WorldLink "Component:WorldLink")** | The world link to open upon touch. |

Fields
Collapse

## Usage

Attach to a slot with a static collider, and provide a `WorldLink` for this to link to in order for it to work.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:TouchWorldLink&oldid=95767](https://wiki.resonite.com/index.php?title=Component:TouchWorldLink&oldid=95767)"

Contents