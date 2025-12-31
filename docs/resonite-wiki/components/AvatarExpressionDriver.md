# Component:AvatarExpressionDriver

> Source: https://wiki.resonite.com/Component:AvatarExpressionDriver

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:AvatarExpressionDriver&diff=98330) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/f/fc/AvatarExpressionDriverComponent.png/510px-AvatarExpressionDriverComponent.png)](https://wiki.resonite.com/File:AvatarExpressionDriverComponent.png) **AvatarExpressionDriver** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

Allows the assignment of the IMouthTrackingSourceComponent to blendshapes.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `DataSource` | **[IMouthTrackingSourceComponent](https://wiki.resonite.com/Type:IMouthTrackingSourceComponent "Type:IMouthTrackingSourceComponent")** | The component that is providing raw mouth tracking data from a physical or virtual device on a machine. |
| `StrengthMultiplier` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Determines strength of expressions |
| `VolumeSource` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | A volume source like a [Volume Meter](https://wiki.resonite.com/Component:VolumeMeter "Component:VolumeMeter") that is used to determine facial tracking better. |
| `SilenceSource` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | A silence source like the target value of the `Silence` field on a [Direct Viseme Driver](https://wiki.resonite.com/Component:DirectVisemeDriver "Component:DirectVisemeDriver") |
| `ExpressionDrivers` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[AvatarExpressionDriver.ExpressionDriver](https://wiki.resonite.com/Component:AvatarExpressionDriver#ExpressionDriver)** | A list of Expression Drivers that take facial data and drive a float or blendshape with the data. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `AutoAssign:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Assign blendshapes to this component's drivers and create new drivers based on heuristics. |

Triggers
Collapse

## ExpressionDriver

| Name | Type | Description |
| --- | --- | --- |
| `Target` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The blendshape or float to drive with this type of expression |
| `Expression` | **[AvatarExpression](https://wiki.resonite.com/Type:AvatarExpression "Type:AvatarExpression")** | The expression to take from the parent AvatarExpressionDriver and drive `Target` with it. |
| `EstimateIfNotTracked` | **[bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to take a guess to this expression's value if it is not tracked |
| `Min` | **[float](https://wiki.resonite.com/Type:Float "Type:Float")** | The minimum value to drive `Target` to. |
| `Max` | **[float](https://wiki.resonite.com/Type:Float "Type:Float")** | The maximum value to drive `Target` to. |
| `VolumeSupressionStrength` | **[float](https://wiki.resonite.com/Type:Float "Type:Float")** | The amount to reduce the effect on `Target` when the user is speaking. |

Fields

## Expression

The different expressions an [ExpressionDriver](https://wiki.resonite.com/Component:AvatarExpressionDriver#ExpressionDriver) can have when driving any float value (or blendshapes)

This list is ever constantly expanding, and as such will be incomplete for vast periods of time. Feel free to help us fill this table.

| Name | Value | Description |
| --- | --- | --- |
| `Smile` |  | How much the user is smiling on average with mouth open slightly |
| `SmileLeft` |  | How much the left lip corner is going up with mouth open slightly |
| `SmileRight` |  | How much the right lip corner is going up with mouth open slightly |
| `SmirkLeft` |  | How much the left lip corner is curling, estimated if not present. |
| `SmirkRight` |  | How much the right lip corner is curling, estimated if not present. |
| `Frown` |  | How much the user is frowning on average. |
| `FrownLeft` |  | How much the left lip corner is going down |
| `FrownRight` |  | How much the right lip corner is going down |
| `MouthDimple` |  | How much the mouth is squishing inward in a strained frown, estimated if not present. |
| `MouthDimpleLeft` |  | How much the mouth is squishing inward in a strained frown left side, estimated if not present. |
| `MouthDimpleRight` |  | How much the mouth is squishing inward in a strained frown right side, estimated if not present. |
| `TongueOut` |  | How much the user is sticking their tongue out |
| `TongueRaise` |  | How much the user is curling their tongue upwards and out |
| `TongueExtend` |  | How much the user is sticking their tongue out 2 |
| `TongueLeft` |  | How much the user is putting their tongue out to the left |
| `TongueRight` |  | How much the user is putting their tongue out to the right |
| `TongueDown` |  | How much the user is putting their tongue out and downwards |
| `TongueUp` |  | How much the user is putting their tongue out to and upwards |
| `TongueRoll` |  | How much the user is rolling their tongue like a taco shape. |
| `TongueHorizontal` |  | How much the tongue is flattening horizontal |
| `TongueVertical` |  | How much the tongue is squishing vertical |
| `TongueUpLeft` |  | How much the user is putting their tongue out to the left and up |
| `TongueUpRight` |  | How much the user is putting their tongue out to the right and up |
| `TongueDownLeft` |  | How much the user is putting their tongue out to the left and down |
| `TongueDownRight` |  | How much the user is putting their tongue out to the right and down |
| `SmileClosed` |  | How much the user is smiling on average, estimated |
| `SmileClosedLeft` |  | How much the left lip corner is going up, estimated if not present. |
| `SmileClosedRight` |  | How much the right lip corner is going up, estimated if not present. |
| `Grin` |  | How much the user is lifting their upper lip while smiling, estimated if not present. |
| `GrinLeft` |  | How much the user is lifting their upper lip while smiling left side, estimated if not present. |
| `GrinRight` |  | How much the user is lifting their upper lip while smiling right side, estimated if not present. |
| `Angry` |  | How much the user is lifting their lips while frowning, estimated if not present. |
| `CheekPuffLeft` |  | How much the user is puffing out their cheeks left side |
| `CheekPuffRight` |  | How much the user is puffing out their cheeks right side |
| `CheekPuff` |  | How much the user is puffing out their cheeks |
| `CheekSuckLeft` |  | How much the user is pulling in their cheeks left side |
| `CheekSuckRight` |  | How much the user is pulling in their cheeks right side |
| `CheekSuck` |  | How much the user is pulling in their cheeks |
| `CheekRaiseLeft` |  |  |
| `CheekRaiseRight` |  |  |
| `CheekRaise` |  |  |
| `LipRaiseUpperLeft` |  | How much the user is lifting their upper lip left side |
| `LipRaiseUpperRight` |  | How much the user is lifting their upper lip right side |
| `LipRaiseLowerLeft` |  | How much the user is lifting their lower lip left side |
| `LipRaiseLowerRight` |  | How much the user is lifting their lower lip right side |
| `LipRaiseUpper` |  | How much the user is lifting their upper lip |
| `LipRaiseLower` |  | How much the user is lifting their lower lip |
| `LipMoveLeftUpper` |  | How much the user is shifting their upper lip to the left |
| `LipMoveRightUpper` |  | How much the user is shifting their upper lip to the right |
| `LipMoveLeftLower` |  | How much the user is shifting their lower lip to the left |
| `LipMoveRightLower` |  | How much the user is shifting their lower lip to the right |
| `LipMoveHorizontalUpper` |  | How much the user is shifting their upper lip |
| `LipMoveHorizontalLower` |  | How much the user is shifting their lower lip |
| `LipTopLeftOverturn` |  |  |
| `LipTopRightOverturn` |  |  |
| `LipTopOverturn` |  | How much the user is flipping their upper lip upwards like an ape |
| `LipBottomLeftOverturn` |  |  |
| `LipBottomRightOverturn` |  |  |
| `LipBottomOverturn` |  | How much the user is flipping their lower lip downwards like an ape |
| `LipOverlayUpper` |  |  |
| `LipOverlayUpperLeft` |  |  |
| `LipOverlayUpperRight` |  |  |
| `LipUnderlayUpper` |  | How much the user is putting their upper lip under their lower lip |
| `LipUnderlayUpperLeft` |  |  |
| `LipUnderlayUpperRight` |  |  |
| `LipOverlayLower` |  |  |
| `LipOverlayLowerLeft` |  |  |
| `LipOverlayLowerRight` |  |  |
| `LipUnderlayLower` |  | How much the user is putting their lower lip under their upper lip |
| `LipUnderlayLowerLeft` |  |  |
| `LipUnderlayLowerRight` |  |  |
| `LipStretch` |  |  |
| `LipStretchLeft` |  |  |
| `LipStretchRight` |  |  |
| `LipTighten` |  |  |
| `LipTightenLeft` |  |  |
| `LipTightenRight` |  |  |
| `LipsPress` |  |  |
| `LipsPressLeft` |  |  |
| `LipsPressRight` |  |  |
| `JawLeft` |  | How much the user is shifting their lower jaw to the left |
| `JawRight` |  | How much the user is shifting their lower jaw to the right |
| `JawHorizontal` |  | How much the user is shifting their lower jaw horizontally |
| `JawForward` |  | How much the user is shifting their lower jaw forward |
| `JawDown` |  | How much the user is opening their jaw but keeping their mouth closed |
| `JawOpen` |  | How much the user is opening their jaw |
| `Pout` |  | How much the user is making a kissy face |
| `PoutLeft` |  | How much the user is making a kissy face left side |
| `PoutRight` |  | How much the user is making a kissy face right side |
| `NoseWrinkle` |  | How much the user's face muscles are pushing up under the nose, estimated if not present. |
| `NoseWrinkleLeft` |  | How much the user's face muscles are pushing up under the nose left side, estimated if not present. |
| `NoseWrinkleRight` |  | How much the user's face muscles are pushing up under the nose right side, estimated if not present. |
| `ChinRaise` |  | How much the user is pulling up their chin |
| `ChinRaiseBottom` |  | How much the user is pulling up their chin bottom side |
| `ChinRaiseTop` |  | How much the user is pulling up their chin top side |

Values

## Usage

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AvatarExpressionDriver&oldid=98330](https://wiki.resonite.com/index.php?title=Component:AvatarExpressionDriver&oldid=98330)"

Contents