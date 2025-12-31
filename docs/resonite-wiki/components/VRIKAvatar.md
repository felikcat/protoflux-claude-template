# Component:VRIKAvatar

> Source: https://wiki.resonite.com/Component:VRIKAvatar

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:VRIKAvatar&diff=106623) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/a/a6/VRIKAvatarComponent.png/510px-VRIKAvatarComponent.png)](https://wiki.resonite.com/File:VRIKAvatarComponent.png) **VRIKAvatar** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **VRIKAvatar** component is used to drive and control the [VRIK](https://wiki.resonite.com/Component:VRIK "Component:VRIK") component on an [Avatar](https://wiki.resonite.com/Avatar "Avatar").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `IK` | **[VRIK](https://wiki.resonite.com/Component:VRIK "Component:VRIK")** | The VRIK to control. |
| `HeightCompensation` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to scale up or down the user's avatar compared to the tracking points. Think a multiplier to avatar scale vs user root. |
| `AvatarHeight` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The height of the avatar from floor to eyes in meters. |
| `UserResizeThreshold` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much the user has to be different from original scale in percentage before prompting to reset scale. |
| `FeetIgnoreOtherPlayers` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether feet raycasts ignore other users. |
| `FeetCollisionListMode` | **[ListFilterMode](https://wiki.resonite.com/Type:ListFilterMode "Type:ListFilterMode")** | The mode to use for feet raycasting whitelist/blacklist. |
| `FeetCollisionList` | _[list](https://wiki.resonite.com/Type:SyncRefList%601 "Type:SyncRefList`1")_ of **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The list of items to filter to/from raycasting according to `FeetCollisionListMode` |
| `HeadMaxFixDistance` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The maximum distance to allow fixing head position due to bad IK. |
| `ForceUseFeetProxies` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to force the use of Feet proxy/tracker objects. |
| `ForceUsePelvisProxy` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to force the use of Pelvis proxy/tracker objects. |
| `ForceUseChestProxy` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to force the use of Chest proxy/tracker objects. |
| `ForceUseElbowProxies` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to force the use of Elbow proxy/tracker objects. |
| `ForceUseKneeProxies` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to force the use of Knee proxy/tracker objects. |
| `FeetCalibrated` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether or not the feet are calibrated. |
| `PelvisCalibrated` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether or not the pelvis is calibrated. |
| `GroundCheckHeightRatio` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How far to check compared to user height for the floor (unused) |
| `FeetHoverHeight` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The height at which feet should hover in either up or down from rest position when off the floor. |
| `FeetHoverSmoothSpeed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to smooth the feet movement when hovering. |
| `MinFeetTransitionSpeed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The minimum speed at random to transition to different modes. |
| `MaxFeetTransitionSpeed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The maximum speed at random to transition to different modes. |
| `GaitFeetTransitionSpeedMultiplier` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to multiply the user's speed to determine the gait speed. |
| `FeetHoverTilt` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to tilt the feet when hovering. |
| `LeftFootFloatOffset` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | How much to offset the left foot when starting hovering. |
| `RightFootFloatOffset` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | How much to offset the right foot when starting hovering. |
| `LeftFootRootHeight` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to move up the left foot when starting hovering. |
| `RightFootRootHeight` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to move up the right foot when starting hovering. |
| `FootFloatSpeed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How fast the feet should move when hovering. |
| `FootFloatAngleMagnitude` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much the feet angle should change when hovering. |
| `FootFloatOffsetMagnitude` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much the feet should wander from avatar center when hovering. |
| `FeetFloatVelocityForce` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much velocity to apply to the feet hovering simulation when moving. |
| `FeetFloatVelocityDampeningSpeed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to dampen velocity over time for the feet hovering simulation. |
| `MaxFeetVelocityOffset` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The maximum amount that the feet can wander from avatar center. |
| `VelocityAverageRate` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The average amount of velocity the user has while moving in user transform space. |
| `HoverVelocityThreshold` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The threshold for velocity the user needs to be to be hovering. |
| `HorizontalBodyAngle` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The angle required for the user to be considered horizontal for their hips. |
| `SupressWalkAnimationWhenHorizontal` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether or not to suppress the walking animation when the user is horizontal. |
| `AlwaysUseTrackersWhenHorizontal` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether or not to always override and use trackers when the user is horizontal. |
| `Gaits` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[Gait](https://wiki.resonite.com/Component:VRIKAvatar#Gait)** | A list of gaits to use when moving (Now is unused). |
| `GaitTransitionSpeed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How fast to transition between different gaits (Now is unused). |
| `GaitMovementDirectionSmoothSpeed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to smooth the gait feet movement direction (Now is unused). |
| `RigCollidersRadiusRatio` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The ratio between the avatar limb length and collider radius sizes. |
| `LeftHandRotationOffset` | **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The offset for the left hand rotation versus controller rotation. |
| `RightHandRotationOffset` | **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The offset for the right hand rotation versus controller rotation. |
| `CurrentAverageVelocity` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The average amount of velocity the user has while moving in user transform space. |
| `CurrentOnGround` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether or not the user is currently is on the ground. |
| `CurrentGaitIndex` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The current walk animation the user is using (Now is unused). |
| `_locomotionController` | **[LocomotionController](https://wiki.resonite.com/Component:LocomotionController "Component:LocomotionController")** | The current locomotion module the user is using. |
| `_leftHandNode` | **[AvatarPoseNode](https://wiki.resonite.com/Component:AvatarPoseNode "Component:AvatarPoseNode")** | The avatar pose node for posing/IK for the left hand. |
| `_rightHandNode` | **[AvatarPoseNode](https://wiki.resonite.com/Component:AvatarPoseNode "Component:AvatarPoseNode")** | The avatar pose node for posing/IK for the right hand. |
| `_leftElbowNode` | **[AvatarPoseNode](https://wiki.resonite.com/Component:AvatarPoseNode "Component:AvatarPoseNode")** | The avatar pose node for posing/IK for the left elbow. |
| `_rightElbowNode` | **[AvatarPoseNode](https://wiki.resonite.com/Component:AvatarPoseNode "Component:AvatarPoseNode")** | The avatar pose node for posing/IK for the right elbow. |
| `_leftFootNode` | **[AvatarPoseNode](https://wiki.resonite.com/Component:AvatarPoseNode "Component:AvatarPoseNode")** | The avatar pose node for posing/IK for the left foot. |
| `_rightFootNode` | **[AvatarPoseNode](https://wiki.resonite.com/Component:AvatarPoseNode "Component:AvatarPoseNode")** | The avatar pose node for posing/IK for the right foot. |
| `_leftKneeNode` | **[AvatarPoseNode](https://wiki.resonite.com/Component:AvatarPoseNode "Component:AvatarPoseNode")** | The avatar pose node for posing/IK for the left knee. |
| `_rightKneeNode` | **[AvatarPoseNode](https://wiki.resonite.com/Component:AvatarPoseNode "Component:AvatarPoseNode")** | The avatar pose node for posing/IK for the right knee. |
| `_headNode` | **[AvatarPoseNode](https://wiki.resonite.com/Component:AvatarPoseNode "Component:AvatarPoseNode")** | The avatar pose node for posing/IK for the head. |
| `_pelvisNode` | **[AvatarPoseNode](https://wiki.resonite.com/Component:AvatarPoseNode "Component:AvatarPoseNode")** | The avatar pose node for posing/IK for the pelvis. |
| `_chestNode` | **[AvatarPoseNode](https://wiki.resonite.com/Component:AvatarPoseNode "Component:AvatarPoseNode")** | The avatar pose node for posing/IK for the chest. |
| `_headProxy` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The proxy slot for the head. |
| `_pelvisProxy` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The proxy slot for the pelvis. |
| `_chestProxy` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The proxy slot for the chest. |
| `_leftHandProxy` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The proxy slot for the left hand. |
| `_rightHandProxy` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The proxy slot for the right hand. |
| `_leftElbowProxy` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The proxy slot for the left elbow. |
| `_rightElbowProxy` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The proxy slot for the right elbow. |
| `_leftFootProxy` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The proxy slot for the left foot. |
| `_rightFootProxy` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The proxy slot for the right foot. |
| `_leftKneeProxy` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The proxy slot for the left knee. |
| `_rightKneeProxy` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The proxy slot for the right knee. |
| `_leftKneeDefaultProxy` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The default proxy slot for the left knee. |
| `_rightKneeDefaultProxy` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The default proxy slot for the right knee. |
| `_headTargetPos` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to drive for the head position. |
| `_headTargetRot` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The field to drive for the head rotation. |
| `_pelvisTargetPos` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to drive for the pelvis position. |
| `_pelvisTargetRot` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The field to drive for the pelvis rotation. |
| `_chestTargetPos` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to drive for the chest position. |
| `_leftHandTargetPos` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to drive for the left hand position. |
| `_leftHandTargetRot` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The field to drive for the left hand rotation. |
| `_rightHandTargetPos` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to drive for the right hand position. |
| `_rightHandTargetRot` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The field to drive for the right hand rotation. |
| `_leftElbowTargetPos` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to drive for the left elbow position. |
| `_rightElbowTargetPos` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to drive for the left elbow position. |
| `_leftFootTargetPos` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to drive for the left foot position. |
| `_leftFootTargetRot` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The field to drive for the left foot rotation. |
| `_rightFootTargetPos` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to drive for the right foot position. |
| `_rightFootTargetRot` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The field to drive for the right foot position. |
| `_leftKneeTargetPos` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to drive for the left knee position. |
| `_rightKneeTargetPos` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to drive for the right knee position. |
| `_pelvisPositionWeight` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The field to drive for the pelvis position weight. |
| `_pelvisRotationWeight` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The field to drive for the pelvis rotation weight. |
| `_chestWeight` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The field to drive for the chest weight. |
| `_locomotionWeight` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The field to drive for the locomotion weight. |
| `_leftLegPositionWeight` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The field to drive for the left leg position weight. |
| `_leftLegRotationWeight` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The field to drive for the left leg rotation weight. |
| `_rightLegPositionWeight` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The field to drive for the right leg position weight. |
| `_rightLegRotationWeight` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The field to drive for the right leg rotation weight. |
| `_leftKneeBendWeight` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The field to drive for the left knee bend weight. |
| `_rightKneeBendWeight` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The field to drive for the right knee bend weight. |
| `_leftElbowBendWeight` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The field to drive for the left elbow bend weight. |
| `_rightElbowBendWeight` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The field to drive for the right elbow bend weight. |
| `_leftFootOffset` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to drive for the left foot bend weight. |
| `_rightFootOffset` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to drive for the right foot bend weight. |
| `_leftFootRelativeToRoot` | **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The rotation of the left foot relative to the character root. |
| `_rightFootRelativeToRoot` | **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The rotation of the right foot to the character root. |
| `_locomotionOffset` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to drive with the locomotion offset. |
| `_simplifiedColliderEnabled` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | The field to drive with the simplified collider hit box. |
| `_rigCollidersEnabledStates` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[FieldDrive\`1](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >** | The field list to drive with all the complex rig collider enabled states. |
| `_horizontalTrackingLocked` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether or not the horizontal rig tracking is locked. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `FilterAvatarHeadPose()` | **[AvatarHeadPoseFilter](https://wiki.resonite.com/Type:AvatarHeadPoseFilter "Type:AvatarHeadPoseFilter")** | ✓ | Used in a transform override component on the user's head to prevent the view from rotating when it's being simulated by the locomotion system |

Triggers
Collapse

## Gait

This part of the system is no longer used, so documentation may be inaccurate, but there is no longer a way to test this system anymore.

| Name | Type | Description |
| --- | --- | --- |
| `MinimumVelocity` | **[float](https://wiki.resonite.com/Type:Float "Type:Float")** | The minimum velocity required for this gait to take effect. |
| `FeetRange` | **[float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The range in which the feet will attempt steps. |
| `CycleHeightBias` | **[float](https://wiki.resonite.com/Type:Float "Type:Float")** | The amount the feet will be biased to step upwards for step height. |
| `CycleFeetSeparation` | **[float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to separate the feet from each other during the cycle. |
| `CycleGroundRatio` | **[float](https://wiki.resonite.com/Type:Float "Type:Float")** | The amount the feet will take into account the ground for the step height. |
| `FootRaiseBeginHeight` | **[float](https://wiki.resonite.com/Type:Float "Type:Float")** | What point the feet should start at for raising for a step. |
| `FootRaiseEndHeight` | **[float](https://wiki.resonite.com/Type:Float "Type:Float")** | What point the feet should end at for raising for a step. |
| `FootRestAngle` | **[float](https://wiki.resonite.com/Type:Float "Type:Float")** | The angle the feet should be at for rest. |
| `FootRaiseAngle` | **[float](https://wiki.resonite.com/Type:Float "Type:Float")** | The angle a foot should be at when making a step. |
| `FeetAlignmentOffset` | **[float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to offset for feet alignment. |
| `SpeedRatio` | **[float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to speed up the foot at the peak of the step. |
| `FeetSlipRatio` | **[float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much the feet will slip before taking a step. |
| `ForwardOffset` | **[float](https://wiki.resonite.com/Type:Float "Type:Float")** | The offset of the feet forwards or backwards. |

Fields

## Usage

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Examples

Used in avatars.

## See Also

- [Avatar](https://wiki.resonite.com/Avatar "Avatar")
- [Component:VRIK](https://wiki.resonite.com/Component:VRIK "Component:VRIK")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:VRIKAvatar&oldid=106623](https://wiki.resonite.com/index.php?title=Component:VRIKAvatar&oldid=106623)"

Contents