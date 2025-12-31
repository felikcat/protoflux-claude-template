# Component:InteractiveCamera

> Source: https://wiki.resonite.com/Component:InteractiveCamera

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/3/31/InteractiveCameraComponent.png/510px-InteractiveCameraComponent.png)](https://wiki.resonite.com/File:InteractiveCameraComponent.png) **Interactive Camera** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **InteractiveCamera** component is used in the resonite default camera and is a way of easily taking pictures.

See [Camera](https://wiki.resonite.com/Camera "Camera") for more up to date info.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `CameraMode` | **[InteractiveCamera.Mode](https://wiki.resonite.com/Component:InteractiveCamera#Mode)** | The mode the camera is in for taking pictures. |
| `PreviewWidth` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The width in pixels of the preview image on the camera screen. |
| `PreviewHeight` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The height in pixels of the preview image on the camera screen. |
| `RenderWidth` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The output width in pixels of the final picture. |
| `StereoSeparation` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How far apart the left and right eyes should be when taking a stereo picture. |
| `TimerInterval` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How long the timer should be for taking a photo. |
| `TimerEnabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the timer mode for taking pictures is enabled. |
| `LastCaptureTime` | _direct_ **[SyncTime](https://wiki.resonite.com/Type:SyncTime "Type:SyncTime")** | The last time in world seconds that this camera took a picture. |
| `TimerCountIndicator` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | The string field to drive with the amount of seconds remaining in the current picture countdown indicator. |
| `TimerColorIndicator` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color field to drive with the indicator color of the current photo countdown timer. |
| `_timerStartPoint` | _direct_ **[SyncTime](https://wiki.resonite.com/Type:SyncTime "Type:SyncTime")** | The world time in seconds when the user started the photo take timer. |
| `_timerUser` | **[User](https://wiki.resonite.com/Type:User "Type:User")** | The user that is handling taking the photo and doing the timer countdown. |
| `MainCamera` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [Camera](https://wiki.resonite.com/Component:Camera "Component:Camera") >** | The main camera being used to preview photos to the screen and render them. |
| `SecondaryCamera` | **[Camera](https://wiki.resonite.com/Component:Camera "Component:Camera")** | The secondary alt camera being used to take photos and render them to the screen. |
| `PreviewTexture` | **[RenderTextureProvider](https://wiki.resonite.com/Component:RenderTextureProvider "Component:RenderTextureProvider")** | The texture that is being rendered to for the camera screen preview on the back of the camera. |
| `DisplayMaterial` | **[IStereoMaterial](https://wiki.resonite.com/index.php?title=Type:IStereoMaterial&action=edit&redlink=1 "Type:IStereoMaterial (page does not exist)")** | The material being used to display the camera preview. |
| `Format` | **[InteractiveCamera.EncodeFormat](https://wiki.resonite.com/Component:InteractiveCamera#EncodeFormat)** | In what image type to take pictures in. |
| `Quality` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The quality encoding for taken pictures. |
| `SpawnPhotoInWorld` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to spawn taken photos into the world. |
| `PhotoSpawnPoint` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | Where to spawn photos and parent them when they are printed out. |
| `PhotoSpawnSize` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How big to spawn the photos. |
| `PanoramaIndicator` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | the slot that holds the panorama indicator visual. |
| `PanoramaIndicatorSize` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to drive so the camera can change the Panorama indicator visual size. |
| `ObjectTargetSource` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot to shoot a raycast from for selective rendering a camera when doing the selective object mode. |
| `ObjectTargetSourceActive` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | The active field of the object target source Laser visual |
| `ObjectAutoPose` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to automatically adjust the camera to look at the targeted object. |
| `HideLasersOnCapture` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to hide user lasers when taking photos. |
| `CaptureSound` | **[AudioClip](https://wiki.resonite.com/Type:AudioClip "Type:AudioClip")** | The audio clip to play when taking photos. |
| `TimerStartSound` | **[AudioClip](https://wiki.resonite.com/Type:AudioClip "Type:AudioClip")** | The audio to play when a photo countdown timer starts. |
| `TimerCountdownSlowPlayer` | **[AudioClipPlayer](https://wiki.resonite.com/Component:AudioClipPlayer "Component:AudioClipPlayer")** | The audio to play when the photo countdown timer is just starting and is counting down. |
| `TimerCountdownFastPlayer` | **[AudioClipPlayer](https://wiki.resonite.com/Component:AudioClipPlayer "Component:AudioClipPlayer")** | The audio to play as the timer for the photo countdown timer is reaching completion. |
| `TimerCountdownSlowOutput` | **[AudioOutput](https://wiki.resonite.com/Component:AudioOutput "Component:AudioOutput")** | The audio output component that plays the `TimerCountdownSlowPlayer`. |
| `TimerCountdownFastOutput` | **[AudioOutput](https://wiki.resonite.com/Component:AudioOutput "Component:AudioOutput")** | The audio output component that plays the `TimerCountdownFastPlayer`. |
| `PreviewScale` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | How big the preview display above the camera should be. |
| `CameraModelOverride` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | Overrides the text for what kind of camera took a photo generated by this component in the metadata. |
| `FrustumVisual` | **[CameraFrustumMesh](https://wiki.resonite.com/Component:CameraFrustumMesh "Component:CameraFrustumMesh")** | The mesh that is used to show the camera fustrum |
| `DefaultNearClip` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The default nearclip to be used with the camera. |
| `DefaultFarClip` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The default farclip to be used with the camera. |
| `_frustumPosition` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to drive with position of the fustrum visual. |
| `_frustumRotation` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The field to drive with the rotation of the fustrum visual. |
| `_frustumVerticalFOV` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The field to drive with the vertical field view angle of the fustrum mesh. |
| `_frustumHorizontalFOV` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The field to drive with the horizontal field view angle of the fustrum mesh. |
| `_frustumNear` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The field to drive with the nearclip of the fustrum mesh. |
| `_frustumFar` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The field to drive with the farclip of the fustrum mesh. |
| `_leftCamOffset` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to drive with the offset of the left camera for stero images. |
| `_rightCamOffset` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to drive with the offset of the right camera for stero images. |
| `_leftCamOrientation` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The field to drive with the rotation of the left camera for stero images. |
| `_rightCamOrientation` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The field to drive with the rotation of the right camera for stero images. |
| `_cameraRendering` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | The field to drive with whether the main camera should be enabled and rendering. |
| `_secondaryCameraRendering` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | The field to drive with whether the secondary camera should be enabled and rendering. |
| `ExclusiveOperators` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[UserRef](https://wiki.resonite.com/Type:UserRef "Type:UserRef")** | The users that should be excluded from taken photos due to their privacy settings. |
| `ControlActiveFields` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[FieldDrive\`1](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >** | A list of booleans to drive to whether this camera is being auto moved by control rather than manual positioning. |
| `RenderOnlyForUsers` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[UserRef](https://wiki.resonite.com/Type:UserRef "Type:UserRef")** | The users that should only appear in the photo and exlude everyone else. |
| `ForceVisualsOff` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to force this camera's visuals to off. |
| `VisualActiveFields` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[FieldDrive\`1](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >** | A list of boolean fields to drive for the visuals of this camera. |
| `AutoHideProximity` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How close the camera can be before it hides itself for the local user. |
| `ForceEyeAttentionUsers` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[UserRef](https://wiki.resonite.com/Type:UserRef "Type:UserRef")** | The list of users to force their eyes to look at the camera. |
| `SimulatingUser` | _direct_ **[UserRef](https://wiki.resonite.com/Type:UserRef "Type:UserRef")** | The user that is handling the processing for this camera. |
| `DestroyOnUserLeave` | _direct_ **[UserRef](https://wiki.resonite.com/Type:UserRef "Type:UserRef")** | The user that when leaving will trigger the destruction of this camera. |
| `PositioningMode` | **[CameraPositioningMode](https://wiki.resonite.com/Type:CameraPositioningMode "Type:CameraPositioningMode")** | How the camera should position itself. |
| `ActiveAnchor` | **[InteractiveCameraAnchor](https://wiki.resonite.com/Component:InteractiveCameraAnchor "Component:InteractiveCameraAnchor")** | The current camera anchor this camera is on. |
| `AnchorInterpolationSpeed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How fast to move between anchors. |
| `AnchorLinearInterpolation` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the camera should move between anchors in a linear speed fashion. |
| `FrameTargetUser` | _direct_ **[UserRef](https://wiki.resonite.com/Type:UserRef "Type:UserRef")** | The user to frame in the shot. |
| `HeadPointOffset` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | How much to add an offset to a user's head when targeting it. |
| `AnglePosition` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | tilt of the camera side to side |
| `Distance` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How far away to stay from a subject during auto tracking. |
| `HeightOffset` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much offset to add to targeting a user's head vertically. |
| `FirstPersonPitch` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The current first person rotation transform pitch. |
| `FirstPersonRoll` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The current first person rotation transform roll. |
| `FirstPersonOffset` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The offset forward or backwards in first person currently. |
| `GroupIncludeRadius` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How close a user needs to be to others to be in a group. |
| `GroupExcludeRadius` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How far a user needs to move from a group before they are removed as being part of a group. |
| `ForceGroupInclude` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[UserRef](https://wiki.resonite.com/Type:UserRef "Type:UserRef")** | A list of users to force include into the target group. |
| `ForceGroupExclude` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[UserRef](https://wiki.resonite.com/Type:UserRef "Type:UserRef")** | A list of users to force exclude from the target group. |
| `PositionSmoothSpeed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The smooth speed of the camera's position during auto tracking. |
| `AnglePositionSmoothSpeed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The smooth speed of the camera's angle position during auto tracking. |
| `FramingSmoothSpeed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The smooth speed of the camera's position during auto tracking for framing. |
| `WobbleMagnitude` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | How much the camera's position should randomly wobble. |
| `WobbleSeed` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The seed of the randomization algorithm of the camera's wobble. |
| `WobbleSpeed` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | How fast the camera should randomly wobble. |
| `FramingViewportPosition` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | Where to frame the target object in the viewport of the camera rather than the center of the image. |
| `AvoidOcclusion` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to take target player(s) colliders into account when framing users. Can help with clipping off arms or legs. |
| `OcclusionIncludePlayers` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether occlusion should try to keep players in view. |
| `OcclusionIncludeAnyColliders` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the occlusion should include any collider. If false, ignores character colliders. |
| `_positionStream` | **[ValueStream\`1](https://wiki.resonite.com/index.php?title=Type:ValueStream%601&action=edit&redlink=1 "Type:ValueStream`1 (page does not exist)") < [Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3") >** | The stream of the position data for this camera when auto tracking. |
| `_rotationStream` | **[ValueStream\`1](https://wiki.resonite.com/index.php?title=Type:ValueStream%601&action=edit&redlink=1 "Type:ValueStream`1 (page does not exist)") < [FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ") >** | The stream of the rotation data for this camera when auto tracking. |
| `_positionDrive` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to drive for the position of the camera when auto tracking. |
| `_rotationDrive` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The field to drive for the rotation of the camera when auto tracking. |
| `_releasePosition` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The position at the time `_positionDrive` became null. |
| `_releaseRotation` | **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The rotation at the time `_rotationDrive` became null. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `Trigger:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Tells camera to take photo as if the user pressed the picture button themselves. |
| `Capture:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Tells the camera to instantly take a photo. |

Triggers
Collapse

## Mode

| Name | Value | Description |
| --- | --- | --- |
| `Camera2D` | 0 | Normal camera mode. |
| `CameraStereo` | 1 | camera renders a 3d photo with a left and right. |
| `Camera360` | 2 | Camera renders a sphere photo. |
| `CameraObject` | 3 | Camera targets an object and renders only that object on a solid background or skybox. |

Values

## EncodeFormat

| Name | Value | Description |
| --- | --- | --- |
| `PNG` | 0 | Save image as a png. |
| `JPG` | 1 | save image as a jpeg. |
| `WebP` | 2 | save image as a webp. |

Values

## Usage

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Component:Camera](https://wiki.resonite.com/Component:Camera "Component:Camera")
- [Component:InteractiveCameraAnchor](https://wiki.resonite.com/Component:InteractiveCameraAnchor "Component:InteractiveCameraAnchor")
- [Camera](https://wiki.resonite.com/Camera "Camera") for more info.

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:InteractiveCamera&oldid=97963](https://wiki.resonite.com/index.php?title=Component:InteractiveCamera&oldid=97963)"

Contents