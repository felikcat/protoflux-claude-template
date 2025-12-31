# Component:Slider

> Source: https://wiki.resonite.com/Component:Slider

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/1/15/SliderComponent.png/510px-SliderComponent.png)](https://wiki.resonite.com/File:SliderComponent.png) **Slider** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Slider** component allows for an object to be grabbed and moved. See [Usage](https://wiki.resonite.com/Component:Slider#Usage) for more information.

![](https://wiki.resonite.com/images/c/c1/SuggestionIcon.svg)

If you need a 2D slider for [UIX](https://wiki.resonite.com/UIX "UIX") as an element, see the [UIX Slider](https://wiki.resonite.com/Component:Slider%601 "Component:Slider`1") component.


## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `EditModeOnly` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines if this grabbable is effective only in [Edit Mode](https://wiki.resonite.com/Edit_Mode "Edit Mode") |
| `AllowSteal` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Other users can grab the slot this component is attached to. Like a flag in capture the flag. |
| `DropOnDisable` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | The parent slot will be dropped when this component is disabled. |
| `DontDrive` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Write the transforms every game tick, rather than driving it on the local machine and then sending the final value to the host. |
| `AllowOnlyPhysicalGrab` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Only allow grab an object with a physical interaction - remote grabs are not allowed |
| `ActiveUserFilter` | **[ActiveUserHandling](https://wiki.resonite.com/Type:ActiveUserHandling "Type:ActiveUserHandling")** | Changes if this component can be grabbed based on who is the active user if any. |
| `CustomGrabCheck` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[GrabCheck](https://wiki.resonite.com/Type:GrabCheck "Type:GrabCheck")** | _Not Usable inside Resonite_ Requires a mod for interacting with [Sync Delegates](https://wiki.resonite.com/Sync_Delegates "Sync Delegates") |
| `_grabber` | **[Grabber](https://wiki.resonite.com/Component:Grabber "Component:Grabber")** | _Automatically Assigned_, the grabber that is grabbing this component. |
| `_holdSlot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot that is "holding" this slot, but not actually acting as this slider's parent. |
| `_pos` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[Sync\`1](https://wiki.resonite.com/Type:Sync%601 "Type:Sync`1") < [Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3") >** | The field this is currently driving for position. |
| `_rot` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[Sync\`1](https://wiki.resonite.com/Type:Sync%601 "Type:Sync`1") < [FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ") >** | The field this is currently driving for rotation. |
| `_scl` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[Sync\`1](https://wiki.resonite.com/Type:Sync%601 "Type:Sync`1") < [Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3") >** | The field this is currently driving for scale. |
| `__legacyActiveUserRootOnly` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | _Automatically Assigned_ Legacy do not use. Used to handle whether only the active user can grab. Use `ActiveUserFilter` instead! |
| `GrabPriority` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Determines what gets grabbed if several grabbable objects are touching someone's grab sphere. The [IGrabbable](https://wiki.resonite.com/Type:IGrabbable "Type:IGrabbable") with the highest priority will be grabbed first. If the highest priority ties with another [IGrabbable](https://wiki.resonite.com/Type:IGrabbable "Type:IGrabbable"), it will grab both of those and ignore any lower priority [IGrabbables](https://wiki.resonite.com/Type:IGrabbable "Type:IGrabbable"). |
| `Rotatable` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the slider object is rotatable. |
| `Scalable` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the slider is scalable. |
| `Range` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The range that the object is allowed to move position wise. |
| `Origin` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The origin of the range that the object is allowed to move. |
| `MinScale` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The minimum scale the object can be scaled to. |
| `MaxScale` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The maximum scale the object can be scaled to. |
| `VibrationOffset` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The offset of the vibration intensity. |
| `VibrationPreset` | **[VibratePreset](https://wiki.resonite.com/Type:VibratePreset "Type:VibratePreset")** | The preset for triggering vibration with this object. |
| `SnapIncrement` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | What increment the position of this object should snap to, instead of allowing smooth movement. |
| `SnapTime` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The time the object will take to move to a snap position when it snaps. |
| `SnapOnRelease` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Only snap to positions in `SnapPositions` when released rather than always. |
| `SnapPositions` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[Slider.SnapPosition](https://wiki.resonite.com/Component:Slider#SnapPosition)** | Positions to snap to while grabbing or when released. |
| `posOffset` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | How much to offset the slider's position. |
| `rotOffset` | **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | How much to offset the slider's rotation. |
| `scaleReference` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The original scale reference value. |
| `referenceParent` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot that is supposed to be this slider's parent. |

Fields
Collapse

## SnapPosition

| Name | Type | Description |
| --- | --- | --- |
| `Position` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The position to snap to and measure distance from. |
| `MaxDistance` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The distance the slider needs to be under from `Position` in local transforms to snap to it. |

Fields

## Usage

This can be used for NPC pickups, grabbing objects and moving them without parenting under a user, or for sliding doors. this can also be used for physical sliders like on audio boards like mixers.

## Examples

Slider - A useful alternative to Grabbable - by [ProbablePrime](https://wiki.resonite.com/User:ProbablePrime "User:ProbablePrime"):

Load video

YouTube

YouTube might collect personal data. [Privacy Policy](https://www.youtube.com/howyoutubeworks/user-settings/privacy/)

ContinueDismiss

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:Slider&oldid=106562](https://wiki.resonite.com/index.php?title=Component:Slider&oldid=106562)"

Contents