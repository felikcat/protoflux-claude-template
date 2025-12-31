# Component:EyeManager

> Source: https://wiki.resonite.com/Component:EyeManager

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:EyeManager&diff=97485) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/b/b5/EyeManagerComponent.png/510px-EyeManagerComponent.png)](https://wiki.resonite.com/File:EyeManagerComponent.png) **EyeManager** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

> _Eye see you_
>
> — Groxxy

The **Eye Manager** Component is a component that is used for configuring the Eyes of an avatar, Both supporting simulated eye-movement, and real eye tracking using a headset with built in eye tracking sensors such as the HTC Vive pro eye.

This component is automatically set up by default when setting up an avatar with detectable eyes and blink shape keys.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `TargetPoint` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The average point The eyes are trying to look at currently. Simulated or controlled. |
| `LeftEyeTargetPoint` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The point The left eye specifically is looking at. Simulated or controlled. This can be different from `TargetPoint` if `LeftEyeTargetOffset` has a non zero value. |
| `RightEyeTargetPoint` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The point The right eye specifically is looking at. Simulated or controlled. This can be different from `TargetPoint` if `RightEyeTargetOffset` has a non zero value. |
| `LeftEyeClose` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much the left eye is closed currently. Simulated or controlled. |
| `RightEyeClose` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much the right eye is closed currently. Simulated or controlled. |
| `CombinedEyeClose` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | an average of how much both eyes are closed. |
| `LeftEyePupilSizeMillimeters` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | how big the left eye's pupil is in millimeters currently. Simulated or controlled. |
| `RightEyePupilSizeMillimeters` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How big the right eye's pupil is currently. Simulated or controlled. |
| `CombinedEyePupilSizeMillimeters` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The average pupil size of both eyes. Simulated or controlled. |
| `LeftEyeWiden` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | A 0-1 value representing how much the left eye is being wider than rest. Simulated or controlled. |
| `RightEyeWiden` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | A 0-1 value representing how much the right eye is being wider than rest. Simulated or controlled. |
| `CombinedEyeWiden` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | An average of the eyes being widened. Simulated or controlled. |
| `LeftEyeSqueeze` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | A 0-1 value of how scrunched the upper and lower lids are on the left eye. Simulated or controlled. |
| `RightEyeSqueeze` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | A 0-1 value of how scrunched the upper and lower lids are on the right eye. Simulated or controlled. |
| `CombinedEyeSqueeze` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | An average of the squinting of both eyes. Simulated or controlled. |
| `LeftEyeFrown` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The amount that the left eye is frowning according to the eye tracker if it exists. |
| `RightEyeFrown` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The amount that the right eye is frowning according to the eye tracker if it exists. |
| `CombinedEyeFrown` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The average amount of both eyes frowning according to the eye tracker if it exists. |
| `LeftEyeInnerBrowVertical` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Eye tracking left inner brow vertical value. |
| `RightEyeInnerBrowVertical` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Eye tracking right inner brow vertical value. |
| `CombinedEyeInnerBrowVertical` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Eye tracking average inner brow vertical value. |
| `LeftEyeOuterBrowVertical` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Eye tracking left outer brow vertical value. |
| `RightEyeOuterBrowVertical` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Eye tracking right outer brow vertical value. |
| `CombinedEyeOuterBrowVertical` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Eye tracking average outer brow vertical value. |
| `EyeDataSource` | **[IEyeDataSourceComponent](https://wiki.resonite.com/Type:IEyeDataSourceComponent "Type:IEyeDataSourceComponent")** | Eye tracking data |
| `SimulatingUser` | **[User](https://wiki.resonite.com/Type:User "Type:User")** | Determines the user simulating the eye manager |
| `SimulateOnHost` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines if the eye manager is simulated by the host |
| `IgnoreLocalUserHead` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines if the eye manager should ignore the local user's head |
| `UserHeadWeight` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Weight for looking at other user heads |
| `UserHandWeight` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Weight for looking at hands |
| `GrippingHandWeight` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Weight for looking at hands that are gripping |
| `CameraWeight` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Weight for looking at cameras |
| `ForcedCameraWeight` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Weight for looking at cameras that are forcing eyes to look at it |
| `EyeReference` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | Slot that is used for referencing the origin of eye tracking data |
| `EyeSeparation` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Seperation of the eyes |
| `SaccadeSpeed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Speed the eyes move during saccades (does not affect eye tracking) |
| `LookTargetRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | Slot that the eyes should look at |
| `LookTargetLocalPoint` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The point that the eyes are looking at in local space. |
| `LeftEyeTargetOffset` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The point that the left eye is looking at in global space. |
| `RightEyeTargetOffset` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The point that the right eye is looking at in global space. |
| `LookTargetOffset` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The point between the points both eyes are looking at in global space. |
| `MinRandomSaccadeInterval` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Minimum time in seconds between random saccades |
| `MaxRandomSaccadeInterval` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Maximum time in seconds between random saccades |
| `MinTargetSaccadeInterval` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Minimum time in seconds between Targeting saccades |
| `MaxTargetSaccadeInterval` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Maximum time in seconds between Targeting saccades |
| `MaxRandomSaccadeOffset` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Maximum distance the eyes can randomly saccade off of the center of a target |
| `DefaultAcceptAngle` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Maximum acceptance angle for random objects |
| `DefaultBreakAngle` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Maximum angle before breaking eye contact with random objects |
| `HeadAcceptAngle` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Maximum acceptance angle for Players |
| `HeadBreakAngle` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Maximum angle before breaking eye contact with Players |
| `CameraAcceptAngle` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Maximum acceptance angle for cameras |
| `CameraBreakAngle` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Maximum angle before breaking eye contact with cameras |
| `HandAcceptAngle` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Maximum acceptance angle for hands |
| `HandBreakAngle` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Maximum angle before breaking eye contact with hands |
| `DistanceCompensationExp` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | At higher values, objects further away become easier to be within angle accept. Equation is \[(ObjectAngleToEyeBall) \* (Object Distance)^`DistanceCompensationExp` == new (ObjectAngleToEyeBall)\] |
| `LeftEyeCloseOverride` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Overrides the left eyelid when open |
| `RightEyeCloseOverride` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Overrides the right eyelid when open |
| `MinBlinkInterval` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Minimum interval between blinks in seconds |
| `MaxBlinkInterval` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Maximum interval between blinks in seconds |
| `BlinkMinSpeed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Minimum Speed for blinks |
| `BlinkMaxSpeed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Maximum Speed for blinks |
| `BlinkSpeedSpread` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to scale the randomness of blink speed. Basically to make more extreme values more common. |
| `MinPupilSize` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Minimum pupil size |
| `MaxPupilSize` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Maximum pupil size |
| `PupilSizeNoiseSpeed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How fast the random pupil noise will move |
| `PupilSizeNoiseOffset` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much extra random noise the right eye pupil size will have vs the left one. |
| `EyeTrackingPupilSizeSmoothSpeed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Smooth speed for tracked pupil dilation |
| `MiniExpressionProbability` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | chance for a miniexpression to occur |
| `MiniExpressionInterval` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Interval between attempting to do a miniexpression |
| `MiniExpressions` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[EyeManager.MiniExpression](https://wiki.resonite.com/Component:EyeManager#MiniExpression)** | A list of mini expressions to use when attempting a mini expression. |

Fields
Collapse

## MiniExpression

| Name | Type | Description |
| --- | --- | --- |
| `Weight` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The likelihood of this mini expression of being picked. |
| `Direction` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The direction to look for this eye expression. |
| `MinDuration` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The minimum amount of seconds this mini expression should last. |
| `MaxDuration` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The maximum amount of seconds this mini expression should last. |

Fields

## Usage

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Component:EyeLinearDriver](https://wiki.resonite.com/Component:EyeLinearDriver "Component:EyeLinearDriver")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:EyeManager&oldid=97485](https://wiki.resonite.com/index.php?title=Component:EyeManager&oldid=97485)"

Contents