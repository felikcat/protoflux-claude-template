# Component:FullBodyCalibrator

> Source: https://wiki.resonite.com/Component:FullBodyCalibrator

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/0/0f/FullBodyCalibratorComponent.png/510px-FullBodyCalibratorComponent.png)](https://wiki.resonite.com/File:FullBodyCalibratorComponent.png) **Full Body Calibrator** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

See [Full Body Tracking](https://wiki.resonite.com/Full_Body_Tracking "Full Body Tracking").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `TargetUser` | **[User](https://wiki.resonite.com/Type:User "Type:User")** | The user we are doing full body tracking for. |
| `UseSymmetryForTrackers` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether changes to sided points (left versus right) mirror onto the other side for the User Calibration Reference. |
| `UseSymmetryForAvatar` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether changes to sided points (left versus right) mirror onto the other side for the Avatar Calibration. |
| `ShowBodyOverlay` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to show the User Calibration Reference. |
| `ShowAvatarOverlay` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to show the avatar reference. |
| `HeightCompensation` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The user height field. |
| `AvatarHeightCompensation` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to multiply the avatar size relative to the User Calibration Reference. |
| `_calibratingPose` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether we are Calibrating the pose or not. |
| `_spaceOffset` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | How much to offset play space. |
| `_grabbable` | **[Grabbable](https://wiki.resonite.com/Component:Grabbable "Component:Grabbable")** | The grabbable Component of the base plate. |
| `_headReference` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The reference visual for the head. |
| `_leftHandReference` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The reference visual for the left hand. |
| `_rightHandReference` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The reference visual for the right hand. |
| `_hipsSource` | **[TrackedDevicePositioner](https://wiki.resonite.com/Component:TrackedDevicePositioner "Component:TrackedDevicePositioner")** | The source of the hips data. |
| `_chestSource` | **[TrackedDevicePositioner](https://wiki.resonite.com/Component:TrackedDevicePositioner "Component:TrackedDevicePositioner")** | The source of the chest data. |
| `_leftFootSource` | **[TrackedDevicePositioner](https://wiki.resonite.com/Component:TrackedDevicePositioner "Component:TrackedDevicePositioner")** | The source of the left foot data. |
| `_rightFootSource` | **[TrackedDevicePositioner](https://wiki.resonite.com/Component:TrackedDevicePositioner "Component:TrackedDevicePositioner")** | The source of the right foot data. |
| `_leftElbowSource` | **[TrackedDevicePositioner](https://wiki.resonite.com/Component:TrackedDevicePositioner "Component:TrackedDevicePositioner")** | The source of the left elbow data. |
| `_rightElbowSource` | **[TrackedDevicePositioner](https://wiki.resonite.com/Component:TrackedDevicePositioner "Component:TrackedDevicePositioner")** | The source of the right elbow data. |
| `_leftKneeSource` | **[TrackedDevicePositioner](https://wiki.resonite.com/Component:TrackedDevicePositioner "Component:TrackedDevicePositioner")** | The source of the left knee data. |
| `_rightKneeSource` | **[TrackedDevicePositioner](https://wiki.resonite.com/Component:TrackedDevicePositioner "Component:TrackedDevicePositioner")** | The source of the right knee data. |
| `_dialog` | **[FullBodyCalibratorDialog](https://wiki.resonite.com/Component:FullBodyCalibratorDialog "Component:FullBodyCalibratorDialog")** | The dialog used to control this full body Calibration interface. |
| `_platformBody` | _direct_ **[FullBodyCalibrator.BodyReference](https://wiki.resonite.com/Component:FullBodyCalibrator#BodyReference)** | The reference on the platform visual. |
| `_userBody` | _direct_ **[FullBodyCalibrator.BodyReference](https://wiki.resonite.com/Component:FullBodyCalibrator#BodyReference)** | The reference on the user in world space. |
| `_customAvatar` | _direct_ **[FullBodyCalibrator.BodyReference](https://wiki.resonite.com/Component:FullBodyCalibrator#BodyReference)** | The custom avatar reference on the platform visual. |
| `_leftHandOverride` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The override slot of the left hand. |
| `_rightHandOverride` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The override slot of the right hand. |
| `_targetCustomAvatar` | **[VRIKAvatar](https://wiki.resonite.com/Component:VRIKAvatar "Component:VRIKAvatar")** | The custom avatar to edit when calibrating the avatar. |
| `_avatarHipsOffset` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The "Target" slot of the avatar hips. |
| `_avatarLeftFootOffset` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The "Target" slot of the avatar left foot. |
| `_avatarRightFootOffset` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The "Target" slot of the avatar right foot. |
| `_avatarLeftKneeDefaultOffset` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The "Target" slot of the avatar left knee. |
| `_avatarRightKneeDefaultOffset` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The "Target" slot of the avatar right knee. |
| `_avatarHipHandle` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The handle object being used to adjust the avatar's hips. |
| `_avatarLeftFootHandle` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The handle object being used to adjust the avatar's left foot. |
| `_avatarRightFootHandle` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The handle object being used to adjust the avatar's right foot. |
| `_avatarLeftKneeHandle` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The handle object being used to adjust the avatar's left knee. |
| `_avatarRightKneeHandle` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The handle object being used to adjust the avatar's right knee. |
| `_avatarLeftKneeOffset` | _direct_ **[FieldHook\`1](https://wiki.resonite.com/index.php?title=Type:FieldHook%601&action=edit&redlink=1 "Type:FieldHook`1 (page does not exist)") < [Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3") >** | The field to hook and change for the left knee offset. |
| `_avatarRightKneeOffset` | _direct_ **[FieldHook\`1](https://wiki.resonite.com/index.php?title=Type:FieldHook%601&action=edit&redlink=1 "Type:FieldHook`1 (page does not exist)") < [Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3") >** | The field to hook and change for the right knee offset. |
| `_platformBodyMaterialSets` | _[list](https://wiki.resonite.com/Type:SyncRefList%601 "Type:SyncRefList`1")_ of **[MaterialSet](https://wiki.resonite.com/Component:MaterialSet "Component:MaterialSet")** | The set of material switchers used to change the platform Body look. |
| `_ground` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The Calibrator platform root slot. |
| `_trackers` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[FullBodyCalibrator.Tracker](https://wiki.resonite.com/Component:FullBodyCalibrator#Tracker)** | A list of trackers registered to the calibrating user. |
| `_visualizationRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot used to store the visuals on the Calibrator platform. |
| `_bodyNodeMaterial` | **[FresnelMaterial](https://wiki.resonite.com/Component:FresnelMaterial "Component:FresnelMaterial")** | The material being used for the visual of the User Calibration Reference. |
| `_calibrationReferenceMaterial` | **[OverlayFresnelMaterial](https://wiki.resonite.com/Component:OverlayFresnelMaterial "Component:OverlayFresnelMaterial")** | The material being used for the visual of the User Calibration Reference. |
| `_leftHandOverrideMaterial` | **[OverlayFresnelMaterial](https://wiki.resonite.com/Component:OverlayFresnelMaterial "Component:OverlayFresnelMaterial")** | The override material for the left hand visual. |
| `_rightHandOverrideMaterial` | **[OverlayFresnelMaterial](https://wiki.resonite.com/Component:OverlayFresnelMaterial "Component:OverlayFresnelMaterial")** | The override material for the right hand visual. |
| `_leftHandOverrideFrontColor` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | the color field for the front color of `_leftHandOverrideMaterial` |
| `_leftHandOverrideBehindColor` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | the color field for the behind color of `_leftHandOverrideMaterial` |
| `_rightHandOverrideFrontColor` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | the color field for the front color of `_rightHandOverrideMaterial` |
| `_rightHandOverrideBehindColor` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | the color field for the behind color of `_rightHandOverrideMaterial` |
| `_patternTex` | **[StaticTexture2D](https://wiki.resonite.com/Component:StaticTexture2D "Component:StaticTexture2D")** | The pattern texture used for the holographic visual for the User Calibration Reference. |
| `_title` | **[TextRenderer](https://wiki.resonite.com/Component:TextRenderer "Component:TextRenderer")** | The title visual of the calibrator pedestal. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `OnRotateLeft:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Handles when the user presses the rotate left button on the platform. |
| `OnRotateRight:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Handles when the user presses the rotate right button on the platform. |
| `OnGrabbableToggle:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Handles when the user presses the grabbable toggle button on the platform. |

Triggers
Collapse

## BodyReference

| Name | Type | Description |
| --- | --- | --- |
| `_vrIkAvatar` | **[VRIKAvatar](https://wiki.resonite.com/Component:VRIKAvatar "Component:VRIKAvatar")** | The VRIK avatar this is getting info from. |
| `_head` | **[IAvatarObject](https://wiki.resonite.com/index.php?title=Type:IAvatarObject&action=edit&redlink=1 "Type:IAvatarObject (page does not exist)")** | The head Avatar object. |
| `_hips` | **[IAvatarObject](https://wiki.resonite.com/index.php?title=Type:IAvatarObject&action=edit&redlink=1 "Type:IAvatarObject (page does not exist)")** | The hips Avatar object. |
| `_chest` | **[IAvatarObject](https://wiki.resonite.com/index.php?title=Type:IAvatarObject&action=edit&redlink=1 "Type:IAvatarObject (page does not exist)")** | The chest Avatar object. |
| `_leftHand` | **[IAvatarObject](https://wiki.resonite.com/index.php?title=Type:IAvatarObject&action=edit&redlink=1 "Type:IAvatarObject (page does not exist)")** | The left hand Avatar object. |
| `_rightHand` | **[IAvatarObject](https://wiki.resonite.com/index.php?title=Type:IAvatarObject&action=edit&redlink=1 "Type:IAvatarObject (page does not exist)")** | The right hand Avatar object. |
| `_leftElbow` | **[IAvatarObject](https://wiki.resonite.com/index.php?title=Type:IAvatarObject&action=edit&redlink=1 "Type:IAvatarObject (page does not exist)")** | The left elbow Avatar object. |
| `_rightElbow` | **[IAvatarObject](https://wiki.resonite.com/index.php?title=Type:IAvatarObject&action=edit&redlink=1 "Type:IAvatarObject (page does not exist)")** | The right elbow Avatar object. |
| `_leftFoot` | **[IAvatarObject](https://wiki.resonite.com/index.php?title=Type:IAvatarObject&action=edit&redlink=1 "Type:IAvatarObject (page does not exist)")** | The left foot Avatar object. |
| `_rightFoot` | **[IAvatarObject](https://wiki.resonite.com/index.php?title=Type:IAvatarObject&action=edit&redlink=1 "Type:IAvatarObject (page does not exist)")** | The right foot Avatar object. |
| `_leftKnee` | **[IAvatarObject](https://wiki.resonite.com/index.php?title=Type:IAvatarObject&action=edit&redlink=1 "Type:IAvatarObject (page does not exist)")** | The left knee Avatar object. |
| `_rightKnee` | **[IAvatarObject](https://wiki.resonite.com/index.php?title=Type:IAvatarObject&action=edit&redlink=1 "Type:IAvatarObject (page does not exist)")** | The right knee Avatar object. |
| `_headPos` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to drive to create the position of the head slot. |
| `_headRot` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The field to drive to create the rotation of the head slot. |
| `_leftHandPos` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to drive to create the position of the left hand slot. |
| `_leftHandRot` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The field to drive to create the rotation of the left hand slot. |
| `_rightHandPos` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to drive to create the position of the right hand slot. |
| `_rightHandRot` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The field to drive to create the rotation of the right hand slot. |
| `_hipsPos` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to drive to create the position of the hips slot. |
| `_hipsRot` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The field to drive to create the rotation of the hips slot. |
| `_chestPos` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to drive to create the position of the chest slot. |
| `_chestRot` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The field to drive to create the rotation of the chest slot. |
| `_leftFootPos` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to drive to create the position of the left foot slot. |
| `_leftFootRot` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The field to drive to create the rotation of the left foot slot. |
| `_rightFootPos` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to drive to create the position of the right foot slot. |
| `_rightFootRot` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The field to drive to create the rotation of the right foot slot. |
| `_leftKneePos` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to drive to create the position of the left knee slot. |
| `_leftKneeRot` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The field to drive to create the rotation of the left knee slot. |
| `_rightKneePos` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to drive to create the position of the right knee slot. |
| `_rightKneeRot` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The field to drive to create the rotation of the right knee slot. |
| `_leftElbowPos` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to drive to create the position of the left elbow slot. |
| `_leftElbowRot` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The field to drive to create the rotation of the left elbow slot. |
| `_rightElbowPos` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to drive to create the position of the right elbow slot. |
| `_rightElbowRot` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The field to drive to create the rotation of the right elbow slot. |
| `_ikWeight` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The Ik weight field of the VRIK. |

Fields

## Tracker

| Name | Type | Description |
| --- | --- | --- |
| `VisualRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The root of the tracker visual. |
| `TrackingReference` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot being used as a tracker position reference. |
| `TrackedDevice` | **[TrackedDevicePositioner](https://wiki.resonite.com/Component:TrackedDevicePositioner "Component:TrackedDevicePositioner")** | The tracker this tracker visual represents. |
| `Material` | **[OverlayFresnelMaterial](https://wiki.resonite.com/Component:OverlayFresnelMaterial "Component:OverlayFresnelMaterial")** | The tracker visual material. |
| `Label` | **[TextRenderer](https://wiki.resonite.com/Component:TextRenderer "Component:TextRenderer")** | The tracker label visual. |
| `CalibrationReference` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The Calibration Reference slot for this tracker. |
| `_position` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The position field of the tracker. |
| `_rotation` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The rotation field of the tracker. |
| `_labelPosition` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The position field of the tracker label. |
| `_labelRotation` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The Rotation field of the tracker label. |

Fields

## Usage

See [Full Body Tracking](https://wiki.resonite.com/Full_Body_Tracking "Full Body Tracking").

## Examples

See [Full Body Tracking](https://wiki.resonite.com/Full_Body_Tracking "Full Body Tracking").

## See Also

- [Full Body Tracking](https://wiki.resonite.com/Full_Body_Tracking "Full Body Tracking")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:FullBodyCalibrator&oldid=98760](https://wiki.resonite.com/index.php?title=Component:FullBodyCalibrator&oldid=98760)"

Contents