# Component:TouchableData

> Source: https://wiki.resonite.com/Component:TouchableData

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:TouchableData&diff=95768) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/a/a4/TouchableDataComponent.png/510px-TouchableDataComponent.png)](https://wiki.resonite.com/File:TouchableDataComponent.png) **Touchable Data** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **TouchableData** component can be used to create simple touch based interactions.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Hovering` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether a user's laser is hovering over the component's collider |
| `Touching` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether a user is clicking on the collider this component is on. |
| `AcceptOutOfSightTouch` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether or not to allow interaction with this component if it is out of the user's view. |
| `AcceptPhysicalTouch` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to allow [Component:TipTouchSources](https://wiki.resonite.com/Component:TipTouchSource "Component:TipTouchSource") to interact with/activate this component. |
| `AcceptRemoteTouch` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this component allows interaction via the user's interaction laser. |
| `OnHoverStartVibrate` | **[VibratePreset](https://wiki.resonite.com/Type:VibratePreset "Type:VibratePreset")** | How to vibrate the user's controller when they started hovering on the component. |
| `OnHoverStayVibrate` | **[VibratePreset](https://wiki.resonite.com/Type:VibratePreset "Type:VibratePreset")** | How to vibrate the user's controller every game update when they are hovering on the component. |
| `OnHoverEndVibrate` | **[VibratePreset](https://wiki.resonite.com/Type:VibratePreset "Type:VibratePreset")** | How to vibrate the user's controller when they stopped hovering on the component. |
| `OnTouchStartVibrate` | **[VibratePreset](https://wiki.resonite.com/Type:VibratePreset "Type:VibratePreset")** | How to vibrate the user's controller when they started primary pressing on the component. |
| `OnTouchStayVibrate` | **[VibratePreset](https://wiki.resonite.com/Type:VibratePreset "Type:VibratePreset")** | How to vibrate the user's controller every game update when they hold primary press on the component. |
| `OnTouchEndVibrate` | **[VibratePreset](https://wiki.resonite.com/Type:VibratePreset "Type:VibratePreset")** | How to vibrate the user's controller when they ended primary pressing on the component. |
| `EditModeOnly` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this component can only be interacted with by users in edit mode. |
| `ActiveUserFilter` | **[ActiveUserHandling](https://wiki.resonite.com/Type:ActiveUserHandling "Type:ActiveUserHandling")** | How to handle which users can use this component based on the current active user. |

Fields
Collapse

## Usage

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Examples

- [Using TouchableData for simple touch based interactions](https://www.youtube.com/watch?v=0cbWeewy3k0) by [ProbablePrime](https://wiki.resonite.com/User:ProbablePrime "User:ProbablePrime")

## See Also

- [Component:TouchButton](https://wiki.resonite.com/Component:TouchButton "Component:TouchButton")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:TouchableData&oldid=95768](https://wiki.resonite.com/index.php?title=Component:TouchableData&oldid=95768)"

Contents