# Component:EyeLinearDriver

> Source: https://wiki.resonite.com/Component:EyeLinearDriver

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:EyeLinearDriver&diff=112774) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/2/2f/EyeLinearDriverComponent.png/510px-EyeLinearDriverComponent.png)](https://wiki.resonite.com/File:EyeLinearDriverComponent.png) **Eye Linear Driver** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **EyeLinearDriver** component is used to drive the shapekeys on eyes. It can also do eye look direction shapekeys if each eye is provided a projection plane slot.

This component can also be used to drive position offsets for eyes. This can be used to make 2D texture based eyes or anime eyes work without needing to use rotation. Please see [How Projection Plane Works](https://wiki.resonite.com/Component:EyeLinearDriver#How_Projection_Plane_Works).

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `EyeManager` | **[EyeManager](https://wiki.resonite.com/Component:EyeManager "Component:EyeManager")** | The eye manager to get the eye data from. |
| `ProjectionPlaneSize` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The scaling of the inital hit point before it is clamped. See [How Projection Plane Works](https://wiki.resonite.com/Component:EyeLinearDriver#How_Projection_Plane_Works). |
| `ProjectionPointDistance` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The distance from the offseted plane to `ProjectionPlanePoint` on all the eyes in `Eyes` list. See [How Projection Plane Works](https://wiki.resonite.com/Component:EyeLinearDriver#How_Projection_Plane_Works). |
| `PositionOffsetCenter` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | How much to add to the inital plane projection hit point after clamping. See [How Projection Plane Works](https://wiki.resonite.com/Component:EyeLinearDriver#How_Projection_Plane_Works). |
| `PositionOffsetRange` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | how much to scale the inital plane projection hit after clamping. See [How Projection Plane Works](https://wiki.resonite.com/Component:EyeLinearDriver#How_Projection_Plane_Works). |
| `MinimumTargetPointDistance` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The minimum distance for every eye in `Eyes` a look target point from that eye's projection plane slot can be. Points closer than that are set to be further than this value during calculation. See [How Projection Plane Works](https://wiki.resonite.com/Component:EyeLinearDriver#How_Projection_Plane_Works). |
| `PositionClampMode` | **[EyeLinearDriver.ClampMode](https://wiki.resonite.com/Component:EyeLinearDriver#ClampMode)** | How to clamp projection plane projection range when doing projection calculations. See [How Projection Plane Works](https://wiki.resonite.com/Component:EyeLinearDriver#How_Projection_Plane_Works). |
| `LeftCloseSubtractLimits` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[EyeLinearDriver.EyeCloseLimit](https://wiki.resonite.com/Component:EyeLinearDriver#EyeCloseLimit)** | The component finds the EyeCloseLimit with the maximum influence in this list. If the EyeCloseLimit with the maximum influence in `CombinedEyeCloseSubtractLimits` is higher, then that is used instead. Then this subtracts the result from the Left Eye close amount (essentially prying the eye open) to get the eye closed value to use with every left eye. |
| `RightCloseSubtractLimits` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[EyeLinearDriver.EyeCloseLimit](https://wiki.resonite.com/Component:EyeLinearDriver#EyeCloseLimit)** | The component finds the EyeCloseLimit with the maximum influence in this list. If the EyeCloseLimit with the maximum influence in `CombinedEyeCloseSubtractLimits` is higher, then that is used instead. Then this subtracts the result from the Left Eye close amount (essentially prying the eye open) to get the eye closed value to use with every right eye. |
| `CombinedCloseSubtractLimits` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[EyeLinearDriver.EyeCloseLimit](https://wiki.resonite.com/Component:EyeLinearDriver#EyeCloseLimit)** | Used with `LeftCloseSubtractLimits` and `RightCloseSubtractLimits` calculations. |
| `Eyes` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[EyeLinearDriver.Eye](https://wiki.resonite.com/Component:EyeLinearDriver#Eye)** | The list of eyes this component is doing calculations and shapekey driving for. |

Fields
Collapse

## Eye

| Name | Type | Description |
| --- | --- | --- |
| `Side` | **[EyeSide](https://wiki.resonite.com/Type:EyeSide "Type:EyeSide")** | The side to get data from for this Eye like target look point and |
| `ProjectionPlanePoint` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot to use as a reference for doing Projection with. See [How Projection Plane Works](https://wiki.resonite.com/Component:EyeLinearDriver#How_Projection_Plane_Works). |
| `PositionOffset` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The field to drive with the final value from the [Projection system](https://wiki.resonite.com/Component:EyeLinearDriver#How_Projection_Plane_Works) for fields like slot position or a 2D texture offset on a material. |
| `LookLeft` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Used to drive the surrounding eye surface shifting when the user looks left for this Eye. See [Eye Look Calculation](https://wiki.resonite.com/Component:EyeLinearDriver#Eye_Look_Calculation). |
| `LookUp` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Used to drive the surrounding eye surface shifting when the user looks up for this Eye. See [Eye Look Calculation](https://wiki.resonite.com/Component:EyeLinearDriver#Eye_Look_Calculation). |
| `LookRight` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Used to drive the surrounding eye surface shifting when the user looks right for this Eye. See [Eye Look Calculation](https://wiki.resonite.com/Component:EyeLinearDriver#Eye_Look_Calculation). |
| `LookDown` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Used to drive the surrounding eye surface shifting when the user looks down for this Eye. See [Eye Look Calculation](https://wiki.resonite.com/Component:EyeLinearDriver#Eye_Look_Calculation). |
| `OpenCloseTarget` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The shapekey or value to use when this eye is closed. |
| `PupilSizeTarget` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The shapekey or value to use when the pupil needs to grow. |
| `WidenTarget` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The shapekey to use to make this eye widen like in shock. |
| `SqueezeTarget` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The shapekey or value to use when this eye is squinting. |
| `FrownTarget` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The shapekey or value to use when this eye is making a frown. |
| `InnerBrowRaiseTarget` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The shapekey or value to use for the inner brow raising for this eye. |
| `InnerBrowLowerTarget` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The shapekey or value to use for the inner brow lowering for this eye. |
| `OuterBrowRaiseTarget` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The shapekey or value to use for the outer brow raising for this eye. |
| `OuterBrowLowerTarget` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The shapekey or value to use for the outer brow lowering for this eye. |
| `MinInputCloseness` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The minimum value the eye tracker can output for eye shut amount for this eye. The subtract limits are applied before the value from the eye tracker makes it to this filter. |
| `MaxInputCloseness` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The maximum value the eye tracker can output for eye shut amount for this eye. The subtract limits are applied before the value from the eye tracker makes it to this filter. |
| `OpenState` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The value to drive `OpenCloseTarget` to when the eye tracker is outputting the minimum possible value for eye shut amount. Which `MinInputCloseness` should also be set to the minimum possible value for eye shut amount from the eye tracker. The subtract limits are applied before the value from the eye tracker makes it to this filter. |
| `CloseState` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The value to drive `OpenCloseTarget` to when the eye tracker is outputting the maximum possible value for eye shut amount. Which `MaxInputCloseness` should also be set to the maximum possible value for eye shut amount from the eye tracker. The subtract limits are applied before the value from the eye tracker makes it to this filter. |
| `MinInputPupilSize` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The minimum value the eye tracker can output for pupil size for this eye. |
| `MaxInputPupilSize` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The maximum value the eye tracker can output for pupil size for this eye. |
| `MinOutputPupilSize` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The value to drive `PupilSizeTarget` to when the eye tracker is outputting the minimum possible value for pupil size. Which `MinInputPupilSize` should also be set to the minimum possible value for pupil size from the eye tracker. |
| `MaxOutputPupilSize` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The value to drive `PupilSizeTarget` to when the eye tracker is outputting the maximum possible value for pupil size. Which `MaxInputPupilSize` should also be set to the maximum possible value for pupil size from the eye tracker. |
| `MinInputWiden` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The minimum value the eye tracker can output for widen in shock for this eye. |
| `MaxInputWiden` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The maximum value the eye tracker can output for widen in shock for this eye. |
| `MinOutputWiden` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The value to drive `WidenTarget` to when the eye tracker is outputting the minimum possible value for widen in shock. Which `MinInputWiden` should also be set to the minimum possible value for widen in shock from the eye tracker. |
| `MaxOutputWiden` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The value to drive `WidenTarget` to when the eye tracker is outputting the minimum possible value for widen in shock. Which `MinInputWiden` should also be set to the minimum possible value for widen in shock from the eye tracker. |
| `MinInputSqueeze` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The minimum value the eye tracker can output for squinting for this eye. |
| `MaxInputSqueeze` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The maximum value the eye tracker can output for squinting for this eye. |
| `MinOutputSqueeze` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The value to drive `SqueezeTarget` to when the eye tracker is outputting the minimum possible value for squint. Which `MinInputSqueeze` should also be set to the minimum possible value for squint from the eye tracker. |
| `MaxOutputSqueeze` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The value to drive `SqueezeTarget` to when the eye tracker is outputting the maximum possible value for squint. Which `MaxInputSqueeze` should also be set to the maximum possible value for squint from the eye tracker. |
| `MinInputFrown` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The minimum value the eye tracker can output for frowning for this eye. |
| `MaxInputFrown` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The maximum value the eye tracker can output for frowining for this eye. |
| `MinOutputFrown` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The value to drive `FrownTarget` to when the eye tracker is outputting the minimum possible value for frown. Which `MinInputFrown` should also be set to the minimum possible value for frown from the eye tracker. |
| `MaxOutputFrown` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The value to drive `FrownTarget` to when the eye tracker is outputting the maximum possible value for frown. Which `MaxInputFrown` should also be set to the maximum possible value for frown from the eye tracker. |
| `MinInputInnerBrowRaise` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The minimum value the eye tracker can output for inner brow raising for this eye. |
| `MaxInputInnerBrowRaise` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The maximum value the eye tracker can output for inner brow raising for this eye. |
| `MinOutputInnerBrowRaise` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The value to drive `InnerBrowRaiseTarget` to when the eye tracker is outputting the minimum possible value for inner brow raising. Which `MinInputInnerBrowRaise` should also be set to the minimum possible value for inner brow raising from the eye tracker. |
| `MaxOutputInnerBrowRaise` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The value to drive `InnerBrowRaiseTarget` to when the eye tracker is outputting the maximum possible value for inner brow raising. Which `MaxInputInnerBrowRaise` should also be set to the maximum possible value for inner brow raising from the eye tracker. |
| `MinInputInnerBrowLower` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The minimum value the eye tracker can output for inner brow lowering for this eye. |
| `MaxInputInnerBrowLower` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The maximum value the eye tracker can output for inner brow lowering for this eye. |
| `MinOutputInnerBrowLower` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The value to drive `InnerBrowLowerTarget` to when the eye tracker is outputting the minimum possible value for inner brow lowering. Which `MinInputInnerBrowLower` should also be set to the minimum possible value for inner brow lowering from the eye tracker. |
| `MaxOutputInnerBrowLower` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The value to drive `InnerBrowLowerTarget` to when the eye tracker is outputting the maximum possible value for inner brow lowering. Which `MaxInputInnerBrowLower` should also be set to the maximum possible value for inner brow lowering from the eye tracker. |
| `MinInputOuterBrowRaise` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The minimum value the eye tracker can output for outer brow raising for this eye. |
| `MaxInputOuterBrowRaise` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The maximum value the eye tracker can output for outer brow raising for this eye. |
| `MinOutputOuterBrowRaise` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The value to drive `InnerBrowOuterTarget` to when the eye tracker is outputting the minimum possible value for outer brow raising. Which `MinInputOuterBrowRaise` should also be set to the minimum possible value for outer brow raising from the eye tracker. |
| `MaxOutputOuterBrowRaise` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The value to drive `InnerBrowOuterTarget` to when the eye tracker is outputting the maximum possible value for outer brow raising. Which `MaxInputOuterBrowRaise` should also be set to the maximum possible value for outer brow raising from the eye tracker. |
| `MinInputOuterBrowLower` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The minimum value the eye tracker can output for outer brow lowering for this eye. |
| `MaxInputOuterBrowLower` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The maximum value the eye tracker can output for outer brow lowering for this eye. |
| `MinOutputOuterBrowLower` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The value to drive `InnerBrowOuterTarget` to when the eye tracker is outputting the minimum possible value for outer brow lowering. Which `MinInputOuterBrowLower` should also be set to the minimum possible value for outer brow lowering from the eye tracker. |
| `MaxOutputOuterBrowLower` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The value to drive `InnerBrowOuterTarget` to when the eye tracker is outputting the maximum possible value for outer brow lowering. Which `MaxInputOuterBrowLower` should also be set to the maximum possible value for outer brow lowering from the eye tracker. |
| `LookMultiply` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | See [Eye Look Calculation](https://wiki.resonite.com/Component:EyeLinearDriver#Eye_Look_Calculation). |
| `LookPower` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | See [Eye Look Calculation](https://wiki.resonite.com/Component:EyeLinearDriver#Eye_Look_Calculation). |

Fields

## EyeCloseLimit

| Name | Type | Description |
| --- | --- | --- |
| `Source` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | The value to use as a source for this subtract limit value. |
| `Multiplier` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The multiplier for `Source` before it becomes this entry's subtract limit value. |

Fields

## ClampMode

| Name | Value | Description |
| --- | --- | --- |
| `Circle` | 0 | clamps movement within an oval based on the Projection plane size. |
| `Square` | 1 | clamps movement within a rectangle based on Projection plane size. |

Values

## How Projection Plane Works

When any eye on this component is provided a slot for `ProjectionPlanePoint`, the projection calculations are allowed to work.

For each eye the Calculation is able to be done on, the component shoots a simulated ray from the `ProjectionPlanePoint` to the eye's look target through an offseted plane. The resulting hit point is modified by some of the component's values (See above fields) and then clamped between -1 to 1. Or within a circle if using [ClampMode](https://wiki.resonite.com/Component:EyeLinearDriver#ClampMode) circle. The value is then modifed by some more component fields, before the result drives `PositionOffset`. Which can drive a texture offset or the position of an eyeball slot for 2D eyes.

## Eye Look Calculation

Eye look calculations for an eye don't work if `ProjectionPlanePoint` is null for that eye.

The clamped hit point from [The Projection System](https://wiki.resonite.com/Component:EyeLinearDriver#How_Projection_Plane_Works) is first multiplied with `LookMultiply` and raised to `LookPower` before it is used for calculating `LookLeft`, `LookRight`, `LookUp`, and `LookDown`.

## Usage

Can be used to drive 2D eyeballs, the shapekeys for eyeballs, and look shapekeys using Ray plane intersection calculations within the component.

## Examples

Used in the eye management system added to avatars using the [Avatar Creator](https://wiki.resonite.com/Avatar_Creator "Avatar Creator") if the option for setup eye tracking is enabled.

## See Also

- [Component:EyeManager](https://wiki.resonite.com/Component:EyeManager "Component:EyeManager")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:EyeLinearDriver&oldid=112774](https://wiki.resonite.com/index.php?title=Component:EyeLinearDriver&oldid=112774)"

Contents