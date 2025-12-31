# Component:Joint

> Source: https://wiki.resonite.com/Component:Joint

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:Joint&diff=98944) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/b/bb/JointComponent.png/510px-JointComponent.png)](https://wiki.resonite.com/File:JointComponent.png) **Joint** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The Joint component allows for a slot or object to rotate around a single point, in any direction, or around an axis. Common uses are doors, helmet tops, and dials.

![](https://wiki.resonite.com/images/c/c1/SuggestionIcon.svg)

Joints go in both directions, making it sometimes confusing. Giving the entire door mechanism a parent slot, rotating it max angle degrees, and then halving the max angle will fix this issue.


## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `EditModeOnly` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | User can only interact with the joint in [Edit Mode](https://wiki.resonite.com/Edit_Mode "Edit Mode") |
| `AllowSteal` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether other users can steal the grabbable joint from other players |
| `DropOnDisable` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether the user drops the joint if the object has been disabled |
| `DontDrive` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Write the transforms every game tick, rather than driving it on the local machine and then sending the final value to the host. |
| `AllowOnlyPhysicalGrab` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Only allow grabbing the joint with a physical interaction - remote grabs are not allowed |
| `ActiveUserFilter` | **[ActiveUserHandling](https://wiki.resonite.com/Type:ActiveUserHandling "Type:ActiveUserHandling")** | How to allow or deny users from interacting with this component depending on the active user. |
| `CustomGrabCheck` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[GrabCheck](https://wiki.resonite.com/Type:GrabCheck "Type:GrabCheck")** | A sync delegate that controls whether this object can be grabbed in certain instances. |
| `_grabber` | **[Grabber](https://wiki.resonite.com/Component:Grabber "Component:Grabber")** | The current Grabber component grabbing this joint. |
| `_holdSlot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The current slot holding this joint. |
| `_pos` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[Sync\`1](https://wiki.resonite.com/Type:Sync%601 "Type:Sync`1") < [Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3") >** | The current position field this is driving or influencing. |
| `_rot` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[Sync\`1](https://wiki.resonite.com/Type:Sync%601 "Type:Sync`1") < [FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ") >** | The current rotation field this is driving or influencing. |
| `_scl` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[Sync\`1](https://wiki.resonite.com/Type:Sync%601 "Type:Sync`1") < [Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3") >** | The current scale field this is driving or influencing. |
| `__legacyActiveUserRootOnly` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to use the legacy active user root only behavior. |
| `GrabPriority` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Determines what gets grabbed if several grabbable objects are touching someone's grab sphere. The [IGrabbable](https://wiki.resonite.com/Type:IGrabbable "Type:IGrabbable") with the highest priority will be grabbed first. If the highest priority ties with another [IGrabbable](https://wiki.resonite.com/Type:IGrabbable "Type:IGrabbable"), it will grab both of those and ignore any lower priority [IGrabbables](https://wiki.resonite.com/Type:IGrabbable "Type:IGrabbable"). |
| `MaxSwing` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Maximum amount the joint will Twist during rotation. |
| `MaxTwist` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Maximum amount the joint will rotate in the given axis |
| `Axis` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | Determines which axis the joint rotates on. Is used like a vector. |
| `TwistReferenceAxis` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The reference axis (vector) for twisting. |
| `PositionTwistThresholdAngle` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The angle at which twist will start affecting position of the slot via position twisting. |
| `VibrationAngle` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The angle at which to trigger vibration. |
| `VibrationPreset` | **[VibratePreset](https://wiki.resonite.com/Type:VibratePreset "Type:VibratePreset")** | The kind and intensity of vibration to send to the grabbing controller. |
| `SnapIncrement` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Snap the joint to a multiple of this angle during grabbing. Can be used to simulate "detents" on a rotary switch. |
| `SnapTime` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The time it takes for the joint to lerp towards given `SnapOrientations`. Higher the value the slower it takes |
| `SnapOnRelease` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether the join snaps to given SnapOrientations |
| `SnapOrientations` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[Joint.SnapOrientation](https://wiki.resonite.com/Component:Joint#SnapOrientation)** | A list of snap orientations that the joint can snap to. |
| `origRotation` | **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The resting rotation of the joint. |
| `rotReference` | **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The reference rotation, which is where the joint started. |
| `dirReference` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The direction the joint started. |
| `twistReference` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The position to use for twist calculations |
| `usePositionTwist` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether twist can influence the position of the joint. |

Fields
Collapse

## Usage

## Examples

Here is a video explaining how joints work by making a door (by [Stellanora](https://wiki.resonite.com/index.php?title=User:Stellanora&action=edit&redlink=1 "User:Stellanora (page does not exist)"))

Load video

YouTube

YouTube might collect personal data. [Privacy Policy](https://www.youtube.com/howyoutubeworks/user-settings/privacy/)

ContinueDismiss

Here are some old videos by [ProbablePrime](https://wiki.resonite.com/User:ProbablePrime "User:ProbablePrime")
Using Joint to make A Door Pt. 1

Load video

YouTube

YouTube might collect personal data. [Privacy Policy](https://www.youtube.com/howyoutubeworks/user-settings/privacy/)

ContinueDismiss

Using Joint to make a Door pt.2

Load video

YouTube

YouTube might collect personal data. [Privacy Policy](https://www.youtube.com/howyoutubeworks/user-settings/privacy/)

ContinueDismiss

## See Also

- [Component:Slider](https://wiki.resonite.com/Component:Slider "Component:Slider")
- [Component:KnobControl](https://wiki.resonite.com/Component:KnobControl "Component:KnobControl")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:Joint&oldid=98944](https://wiki.resonite.com/index.php?title=Component:Joint&oldid=98944)"

Contents