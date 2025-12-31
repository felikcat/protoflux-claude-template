# Component:TouchToggle

> Source: https://wiki.resonite.com/Component:TouchToggle

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:TouchToggle&diff=100793) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/f/f7/TouchToggleComponent.png/510px-TouchToggleComponent.png)](https://wiki.resonite.com/File:TouchToggleComponent.png) **Touch Toggle** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **TouchToggle** component acts as a button that works as a check box, and the different Toggle on and off action can be mapped to certain Touch events.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `State` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | The checkbox state of this touch toggle. |
| `EventType` | **[TouchEventType](https://wiki.resonite.com/Type:TouchEventType "Type:TouchEventType")** | the type of touch event to listen for different event states from. |
| `ToggleEvent` | **[EventState](https://wiki.resonite.com/Type:EventState "Type:EventState")** | The event state needed when touching to Toggle the `State` value. |
| `OnEvent` | **[EventState](https://wiki.resonite.com/Type:EventState "Type:EventState")** | The event state needed when touching to switch to true the `State` value. |
| `OffEvent` | **[EventState](https://wiki.resonite.com/Type:EventState "Type:EventState")** | The event state needed when touching to switch to false the `State` value. |
| `AcceptOutOfSightTouch` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether or not to allow interaction with this component if it is out of the user's view. |
| `AcceptPhysicalTouch` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to allow [Component:TipTouchSources](https://wiki.resonite.com/Component:TipTouchSource "Component:TipTouchSource") to interact with/activate this component. |
| `AcceptRemoteTouch` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this component allows interaction via the user's interaction laser. |
| `Vibrate` | **[VibratePreset](https://wiki.resonite.com/Type:VibratePreset "Type:VibratePreset")** | How to vibrate the user's hand when they touch the toggle. |
| `EditModeOnly` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this is only available in edit mode. |
| `ActiveUserFilter` | **[ActiveUserHandling](https://wiki.resonite.com/Type:ActiveUserHandling "Type:ActiveUserHandling")** | how to filter users in the session who can interact with this component depending on the parent user. |
| `__legacyActiveUserRootOnly` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to use the legacy active user root. Internal. |

Fields
Collapse

## Usage

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Examples

- [Doors Pt.3 using TouchToggle and Tween for an automatic Door](https://www.youtube.com/watch?v=zMDpwG4H6sM) by [ProbablePrime](https://wiki.resonite.com/User:ProbablePrime "User:ProbablePrime")

## See Also

- [Type:ITouchable](https://wiki.resonite.com/Type:ITouchable "Type:ITouchable")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:TouchToggle&oldid=100793](https://wiki.resonite.com/index.php?title=Component:TouchToggle&oldid=100793)"

Contents