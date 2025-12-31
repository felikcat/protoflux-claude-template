# Component:VRIK

> Source: https://wiki.resonite.com/Component:VRIK

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/d/dc/VRIK.png/510px-VRIK.png)](https://wiki.resonite.com/File:VRIK.png) **VRIK** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

## Introduction

> _Oof_
>
> — Epsilion

The **VRIK** component is used to configure [Inverse Kinematics](https://wiki.resonite.com/IK "IK") on an avatar, for posing joints based on the position of IK Targets such as a [VR HMD](https://en.wikipedia.org/wiki/Head-mounted_display), [hand tracking](https://en.wikipedia.org/wiki/Hand_tracking), or [Vive Trackers](https://www.vive.com/us/accessory/vive-tracker/)

This component is automatically configured when importing a mesh with a detectable [humanoid rig](https://docs.unity3d.com/Manual/UsingHumanoidChars.html#Rigging), and generally should not be modified unless you know what you are doing.

Documentation on this component may take some time, as it is very complex, and not commonly used. The basis for this component seems to be the VRIK solver developed by [Final IK](http://www.root-motion.com/finalikdox/html/page16.html).

## Usage

All weight values are 1-0, excluding clamps which are inverted 0-1.
You can overdrive some of them with interesting results.

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `AutoUpdate` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to update the VRIK regardless of whether or not the sync delegates are called by a VRIK avatar or similar sources. this can break systems still using a VRIKAvatar but can fix ones with a lack of such component. |
| `FixTransformsEnabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Clamps IK transforms to reasonable values and Resets IK every update. |
| `Solver` | _direct_ **[IKSolverVR](https://wiki.resonite.com/Type:IKSolverVR "Type:IKSolverVR")** | The actual solver that contains most of the fields of this component. |
| `componentInitiated` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Marks this component as fully started and ready to solve IK transforms. |
| `_drives` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[VRIK.BoneDrive](https://wiki.resonite.com/Component:VRIK#BoneDrive)** | A list of fields to drive with `defaultLocalPositions` and `defaultLocalRotations` plus transforms solved by the IK using `defaultLocalPositions` and `defaultLocalRotations` as a basis. |

Fields
Collapse

## IKSolverVR

Most of the complexity in VRIK is actually stored in the **IKSolverVR** type. And even this is spread across multiple types.

| Name | Type | Description |
| --- | --- | --- |
| `IKPosition` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | Unused. |
| `IKPositionWeight` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Weight of the IK. Makes the bones go back to `defaultLocalPositions` and `defaultLocalRotations` as this goes to 0. Also known as default pose. |
| `SimulationSpace` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The top most hiearchy this solver should simulate in. When on an Avatar this is usually the user's slot when equipped and the avatar root when unequipped. |
| `OffsetSpace` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | Is used to determine if there is movement happening in user space. for example shuffling around in the player's physical room. This also tells the feet to try to find new footing, and to tell the feet the user is moving. |
| `_initiated` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether or not this component is simulating and driving it's fields. |
| `OnPreInitiate` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[UpdateDelegate](https://wiki.resonite.com/Type:UpdateDelegate "Type:UpdateDelegate")** | Currently unused. Fires the SyncDelegate inside when this component is started initializing(usually during loading) |
| `OnPostInitiate` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[UpdateDelegate](https://wiki.resonite.com/Type:UpdateDelegate "Type:UpdateDelegate")** | Currently unused. Fires the SyncDelegate inside when this component is done initializing (usually during loading) |
| `OnPreUpdate` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[UpdateDelegate](https://wiki.resonite.com/Type:UpdateDelegate "Type:UpdateDelegate")** | Sync Delegate usually filled with calls to the [VRIKAvatar component](https://wiki.resonite.com/Component:VRIKAvatar "Component:VRIKAvatar"). |
| `OnPostUpdate` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[UpdateDelegate](https://wiki.resonite.com/Type:UpdateDelegate "Type:UpdateDelegate")** | Sync Delegate usually filled with calls to the [VRIKAvatar component](https://wiki.resonite.com/Component:VRIKAvatar "Component:VRIKAvatar"). |
| `root` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The root of the solver simulation, on an avatar this will be the avatar root when equipped and nothing when dequipped. |
| `BoneReferences` | _direct_ **[References](https://wiki.resonite.com/Component:VRIK#References)** | The set of slots are what parts of the VRIK. |
| `defaultLocalPositions` | _[array](https://wiki.resonite.com/Type:SyncArray%601 "Type:SyncArray`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | This is internal, and stores the positions the bones should go to as IKPositionWeight goes to 0. |
| `defaultLocalRotations` | _[array](https://wiki.resonite.com/Type:SyncArray%601 "Type:SyncArray`1")_ of **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | This is internal, and stores the rotations the bones should go to as IKPositionWeight goes to 0. |
| `DebugVisuals` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Enables Debug visuals |
| `PlantFeet` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | When enabled, feet positions will be prioritized over anything else including HeadTarget. (Causes issues with walking) If true, will keep the toes planted even if the HeadTarget is out of reach, so this can cause the camera to exit the head if it is too high for the model to reach. |
| `spine` | _direct_ **[Spine](https://wiki.resonite.com/Component:VRIK#Spine)** | The spine section of the VRIK solver. |
| `leftArm` | _direct_ **[Arm](https://wiki.resonite.com/Component:VRIK#Arm)** | The left arm section of the VRIK solver. |
| `rightArm` | _direct_ **[Arm](https://wiki.resonite.com/Component:VRIK#Arm)** | The right arm section of the VRIK solver. |
| `leftLeg` | _direct_ **[Leg](https://wiki.resonite.com/Component:VRIK#Leg)** | The left leg section of the VRIK solver. |
| `rightLeg` | _direct_ **[Leg](https://wiki.resonite.com/Component:VRIK#Leg)** | The right leg section of the VRIK solver. |
| `locomotion` | _direct_ **[Locomotion](https://wiki.resonite.com/Component:VRIK#Locomotion)** | The locomotion section of the VRIK solver. |
| `ForwardFlipped` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Swaps the feet and turns the whole IK around. |
| `ForceRootHeight` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | Foot planting height override (Negative numbers cause issues with walking) |
| `LocomotionPositionOffset` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | Handles how the IK should be offset when calculating locomotion. |
| `DefaultRootPosition` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The default position of the centered root. |
| `DefaultRootRotation` | **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The default rotation of the centered root. |

Fields

### References

| Name | Type | Description |
| --- | --- | --- |
| `root` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The root of the VRIK, usually avatar root. |
| `pelvis` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | Usually is set to the avatar's mapped `Hips` [BodyNode](https://wiki.resonite.com/Type:BodyNode "Type:BodyNode"). |
| `spine` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | Usually is set to the avatar's mapped `Spine` [BodyNode](https://wiki.resonite.com/Type:BodyNode "Type:BodyNode"). |
| `chest` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | Usually is set to the avatar's mapped `Chest` [BodyNode](https://wiki.resonite.com/Type:BodyNode "Type:BodyNode"). |
| `neck` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | Usually is set to the avatar's mapped `Neck` [BodyNode](https://wiki.resonite.com/Type:BodyNode "Type:BodyNode"). |
| `head` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | Usually is set to the avatar's mapped `Head` [BodyNode](https://wiki.resonite.com/Type:BodyNode "Type:BodyNode"). |
| `leftShoulder` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | Usually is set to the avatar's mapped `LeftShoulder` [BodyNode](https://wiki.resonite.com/Type:BodyNode "Type:BodyNode"). |
| `leftUpperArm` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | Usually is set to the avatar's mapped `LeftUpperArm` [BodyNode](https://wiki.resonite.com/Type:BodyNode "Type:BodyNode"). |
| `leftForearm` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | Usually is set to the avatar's mapped `LeftLowerArm` [BodyNode](https://wiki.resonite.com/Type:BodyNode "Type:BodyNode"). |
| `leftHand` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | Usually is set to the avatar's mapped `LeftHand` [BodyNode](https://wiki.resonite.com/Type:BodyNode "Type:BodyNode"). |
| `rightShoulder` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | Usually is set to the avatar's mapped `RightShoulder` [BodyNode](https://wiki.resonite.com/Type:BodyNode "Type:BodyNode"). |
| `rightUpperArm` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | Usually is set to the avatar's mapped `RightUpperArm` [BodyNode](https://wiki.resonite.com/Type:BodyNode "Type:BodyNode"). |
| `rightForearm` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | Usually is set to the avatar's mapped `RightLowerArm` [BodyNode](https://wiki.resonite.com/Type:BodyNode "Type:BodyNode"). |
| `rightHand` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | Usually is set to the avatar's mapped `RightHand` [BodyNode](https://wiki.resonite.com/Type:BodyNode "Type:BodyNode"). |
| `leftThigh` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | Usually is set to the avatar's mapped `LeftUpperLeg` [BodyNode](https://wiki.resonite.com/Type:BodyNode "Type:BodyNode"). |
| `leftCalf` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | Usually is set to the avatar's mapped `LeftLowerLeg` [BodyNode](https://wiki.resonite.com/Type:BodyNode "Type:BodyNode"). |
| `leftFoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | Usually is set to the avatar's mapped `LeftFoot` [BodyNode](https://wiki.resonite.com/Type:BodyNode "Type:BodyNode"). |
| `leftToes` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | Usually is set to the avatar's mapped `LeftToes` [BodyNode](https://wiki.resonite.com/Type:BodyNode "Type:BodyNode"). |
| `rightThigh` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | Usually is set to the avatar's mapped `RightUpperLeg` [BodyNode](https://wiki.resonite.com/Type:BodyNode "Type:BodyNode"). |
| `rightCalf` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | Usually is set to the avatar's mapped `RightLowerLeg` [BodyNode](https://wiki.resonite.com/Type:BodyNode "Type:BodyNode"). |
| `rightFoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | Usually is set to the avatar's mapped `RightFoot` [BodyNode](https://wiki.resonite.com/Type:BodyNode "Type:BodyNode"). |
| `rightToes` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | Usually is set to the avatar's mapped `RightToes` [BodyNode](https://wiki.resonite.com/Type:BodyNode "Type:BodyNode"). |

Fields

### Spine

| Name | Type | Description |
| --- | --- | --- |
| `Initiated` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether or not the spine section is initalized. |
| `HeadTarget` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | This slot is used to position the `head` when set. When unset the head position is determined by `IKPositionHead` and `IKRotationHead`. |
| `PelvisTarget` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | This slot is used to position the `pelvis` when set. When unset the pelvis position is determined by `IKPositionPelvis` and `IKRotationPelvis`. |
| `PositionWeight` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Positional weight of the HeadTarget. |
| `RotationWeight` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Rotational weight of the HeadTarget. |
| `PelvisPositionWeight` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Positional weight of the PelvisTarget. |
| `PelvisRotationWeight` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Rotational weight of the PelvisTarget. |
| `ChestGoal` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | If ChestGoalWeightis greater than 0, the `chest` will be turned towards this slot when set. When unset, `GoalPositionChest` is used as a position to turn towards. |
| `ChestGoalWeight` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Weight of turning the chest towards the ChestGoal. |
| `MinHeadHeight` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Minimum Head height allowed by the IK solver (Nonfunctional) |
| `BodyPosStiffness` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much the body will try to move with the `HeadTarget` or with `IKPositionHead` and `IKRotationHead` if `HeadTarget` is unset. |
| `BodyRotStiffness` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much the body will try to rotate with the `HeadTarget` or with `IKPositionHead` and `IKRotationHead` if `HeadTarget` is unset. |
| `NeckStiffness` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much the chest will rotate when the head is rotated. |
| `RotateChestByHands` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much the chest rotates based on hand movement. |
| `ChestClampWeight` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much the chest can rotate relative to the head with 0 being full movement and 1 being no movement. A value of 0.5 allows 90 degrees of rotation for the chest relative to the head. A value of 0 allows 180 degrees and a value of 1 means the chest will be locked relative to the head. |
| `HeadClampWeight` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much the head can rotate relative to the `HeadTarget` or with `IKPositionHead` and `IKRotationHead` if `HeadTarget` is unset with 0 being full movement and 1 being no movement. A value of 0.5 allows 90 degrees of rotation for the head relative to the target. A value of 0 allows 180 degrees and a value of 1 means head rotation will be locked to the target. |
| `MoveBodyBackWhenCrouching` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much the body will move backwards when crouching |
| `MaintainPelvisPosition` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much the pelvis will move with the feet instead of the `HeadTarget` or with `IKPositionHead` and `IKRotationHead` if `HeadTarget` is unset. |
| `MaxRootAngle` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much the `HeadTarget` or with `IKPositionHead` and `IKRotationHead` if `HeadTarget` is unset must rotate for the whole body to rotate (in degrees). |
| `IKPositionHead` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The solved position for the head. Driven. |
| `IKRotationHead` | **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The solved rotation for the head. Driven. |
| `IKPositionPelvis` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The solved position for the pelvis. Driven. |
| `IKRotationPelvis` | **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The solved rotation for the pelvis. Driven. |
| `GoalPositionChest` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The solved goal position for the chest. Driven. |
| `headHeight` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Head height while standing. Used for calculating MoveBodyBackWhenCrouching. |
| `anchorRelativeToHead` | **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | Root rotation relative to `HeadTarget` or with `IKPositionHead` and `IKRotationHead` if `HeadTarget` is unset. |
| `pelvisRelativeRotation` | **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | Pelvis rotation relative to `HeadTarget` or with `IKPositionHead` and `IKRotationHead` if `HeadTarget` is unset. |
| `chestRelativeRotation` | **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | Chest rotation relative to `HeadTarget` or with `IKPositionHead` and `IKRotationHead` if `HeadTarget` is unset. |
| `chestForward` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | Chest Forward Vector |
| `pelvisForward` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | Pelvis Forward Vector |

Fields

### Arm

Contains parameters for the two arms: `leftArm` and `rightArm`.

| Name | Type | Description |
| --- | --- | --- |
| `Initiated` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this arm section is initalized. |
| `Target` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The target for the arm's hand. It will use this if set, or `PositionWeight` and `RotationWeight` if unset. |
| `BendGoal` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The arm's elbow will be bent towards this slot if `BendGoalWeight` \> 0, and the slot is set. Otherwise `BendGoalPosition` is used as a bend position. |
| `PositionWeight` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Positional weight of the Target. |
| `RotationWeight` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Rotational weight of the Target. |
| `ShoulderRotationMode` | **[ShoulderRotationMode](https://wiki.resonite.com/Component:VRIK#ShoulderRotationMode)** | Shoulder rotation method. Pitch/yaw is more accurate, while From/to is simpler. |
| `ShoulderRotationWeight` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much the arm's shoulder should move based on Hand position. |
| `BendGoalWeight` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | if greater than 0, will bend the elbow towards the `BendGoal` slot if set otherwise `BendGoalPosition` is used |
| `SwivelOffset` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Rotation offset for the arm's elbow in degrees. |
| `WristToPalmAxis` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | Palm Direction; local axis of the hand bone that points from the wrist towards the palm. Used for defining hand bone orientation. (Higher values on the Y axis increase the amount the arms move with your controllers) |
| `PalmToThumbAxis` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | Thumb Direction; local axis of the hand bone that points from the palm towards the thumb. Used for defining hand bone orientation. |
| `ArmLengthMlp` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Arm Length Multiplier. Used to make the arm shorter/longer. Works by displacement of hand and forearm local position. |
| `StretchCurve` | _direct_ **[SyncCurve\`1](https://wiki.resonite.com/index.php?title=Type:SyncCurve%601&action=edit&redlink=1 "Type:SyncCurve`1 (page does not exist)") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | Unsupported. Would evaluate stretching of the arm by target distance relative to arm length. Value at time 1 represents stretching amount at the point where distance to the target is equal to arm length. Value at time 2 represents stretching amount at the point where distance to the target is double the arm length. Value represents the amount of stretching. Linear stretching would be achieved with a linear curve going up by 45 degrees. Increase the range of stretching by moving the last key up and right at the same amount. Smoothing in the curve can help reduce elbow snapping (start stretching the arm slightly before target distance reaches arm length). |
| `IKPosition` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The solved position for the arm's hand. Driven. |
| `IKRotation` | **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The solved rotation for the arm's hand. Driven. |
| `BendGoalPosition` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The solved position for the bend goal. Driven. |
| `TwistRelaxWeight` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much the forearm twists towards the wrist |
| `TwistCrossfade` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Weight of the forearm twisting |
| `TwistAngleOffset` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Angle offset of the forearm twisting |
| `chestForwardAxis` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The axis used to tell the VRIK what direction the chest is pointing forward by default. usually set when the chest bone roll is different from 0 in blender. |
| `chestUpAxis` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The axis used to tell the VRIK what direction the chest is pointing up by default. usually set when the chest doesn't point directly towards the next bone in the chain. |
| `forearmTwistAxis` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | This specifies what axis the forearms should twist around in local space. |
| `forearmAxis` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | This specifies the axis that the forearm takes place along in local space. |
| `axisRelativeToUpperArm` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | This identifies which axis the forearm is from the upper arm. |
| `axisRelativeToHand` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | This identifies which axis the hand is from the forearm. |

Fields

#### ShoulderRotationMode

| Name | Value | Description |
| --- | --- | --- |
| `YawPitch` | 0 | Rotates the shoulder using Yaw Pitch, which is like using Slerp. |
| `FromTo` | 1 | Rotates the shoulder using essentially a look at, which can solve some IK issues. |

Values

### Leg

Contains parameters for the two legs: `leftLeg` and `rightLeg`.

| Name | Type | Description |
| --- | --- | --- |
| `Initiated` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this leg is initialized. |
| `Target` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The target for the left foot/toe. This can override the `IKPosition` and `IKRotation` values so it uses this slot as a target position instead. |
| `BendGoalPosition` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The solved position for the bend goal. Driven. |
| `BendGoal` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The left knee will be bent towards this slot if BendGoalWeight > 0 if set. otherwise `BendGoalPosition` is used. |
| `PositionWeight` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Positional weight of the Target. |
| `RotationWeight` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Rotational weight of the Target. |
| `BendGoalWeight` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | if greater than 0, will bend the left knee towards the `BendGoal` slot if set otherwise `BendGoalPosition` is used. |
| `SwivelOffset` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Rotation offset for the left knee in degrees. |
| `CalfBendNormal` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The direction the calf should bend towards in local space. |
| `IKPosition` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The solved position for the left foot/toe. Driven. |
| `IKRotation` | **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The solved rotation for the left foot/toe. Driven. |

Fields

### Locomotion

| Name | Type | Description |
| --- | --- | --- |
| `Weight` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much weight locomotion calculation has rather than normal IK calculation. |
| `FootDistance` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Tries to maintain this distance between where each foot will attempt to plant themselves. |
| `StepThreshold` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How far you have to move for the feet to take a step (re-plant themselves). |
| `AngleThreshold` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much you have to rotate for the feet to take a step (re-plant themselves). |
| `ComAngleMlp` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Multiplier angle of the (center of mass minus the center of pressure) vector. Larger value makes the character step sooner if losing balance. |
| `MaxVelocity` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Maximum magnitude of head/hand target velocity for prediction. |
| `VelocityFactor` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much the feet will use your current head/hand target velocity to predict where you're stepping. |
| `MaxLegStretch` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much your leg can stretch before it attempts to take a step. 1 means fully stretched. |
| `RootSpeed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How fast the pelvis and legs will move to catch up to the HMD; the speed of lerping the root of the character towards the horizontal mid-point of the footsteps. |
| `StepSpeed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How fast the foot planter will move the feet to their new position when re-planting |
| `StepHeight` | _direct_ **[SyncCurve\`1](https://wiki.resonite.com/index.php?title=Type:SyncCurve%601&action=edit&redlink=1 "Type:SyncCurve`1 (page does not exist)") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | The height of the foot by normalized step progress (0 - 1). |
| `HeelHeight` | _direct_ **[SyncCurve\`1](https://wiki.resonite.com/index.php?title=Type:SyncCurve%601&action=edit&redlink=1 "Type:SyncCurve`1 (page does not exist)") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | The height offset of the heel by normalized step progress (0 - 1). |
| `RelaxLegTwistMinAngle` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much your HMD has to rotate before your feet begin to rotate towards your HMD without stepping; rotates the foot while the leg is not stepping to relax the twist rotation of the leg if ideal rotation is past this angle. |
| `RelaxLegTwistSpeed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How fast the feet can rotate while on the ground; the speed of rotating the foot while the leg is not stepping to relax the twist rotation of the leg. |
| `StepInterpolation` | **[InterpolationMode](https://wiki.resonite.com/Type:InterpolationMode "Type:InterpolationMode")** | The type of interpolation the feet will use during stepping. |
| `Offset` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | Offset for feet planting relative to your HMD |
| `LeftFootOffset` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | How much to offset the foot from the given target position and rotation for the left foot. |
| `RightFootOffset` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | How much to offset the foot from the given target position and rotation for the right foot. |
| `OnLeftFootstep` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | This is very finicky, and can be used to fire sounds or other Action sync delegates when the left foot steps. |
| `OnRightFootstep` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | This is very finicky, and can be used to fire sounds or other Action sync delegates when the right foot steps. |
| `_leftFootstep` | _direct_ **[Footstep](https://wiki.resonite.com/Component:VRIK#Footstep)** | A list of footsteps to trigger for the left foot. |
| `_rightFootstep` | _direct_ **[Footstep](https://wiki.resonite.com/Component:VRIK#Footstep)** | A list of footsteps to trigger for the right foot. |

Fields

### Footstep

| Name | Type | Description |
| --- | --- | --- |
| `_initialized` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this footstep should be used. |
| `footRelativeToRoot` | **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The rotation relative to root needed for this to be considered a footstep. |
| `footGroundHeight` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The height needed for this to be considered a footstep. |

Fields

## BoneDrive

Bonedrive fields use a combination of the `defaultLocalPositions` and `defaultLocalRotations` entries at this element's entry position in the list as well as VRIK position and rotation solved values to determine the final driven value.

| Name | Type | Description |
| --- | --- | --- |
| `Position` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to drive with the VRIK's solved position for the bone that corrosponds to this entry. |
| `Rotation` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The field to drive with the VRIK's solved rotation for the bone that corrosponds to this entry. |

Fields

## Usage

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Examples

Used in every avatar except head and hands avatars to make avatar movements.

## See Also

- [Component:VRIKAvatar](https://wiki.resonite.com/Component:VRIKAvatar "Component:VRIKAvatar")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:VRIK&oldid=100822](https://wiki.resonite.com/index.php?title=Component:VRIK&oldid=100822)"

Contents