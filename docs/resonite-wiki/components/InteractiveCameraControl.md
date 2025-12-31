# Component:InteractiveCameraControl

> Source: https://wiki.resonite.com/Component:InteractiveCameraControl

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This is a **[userspace](https://wiki.resonite.com/Userspace "Userspace") component** — you cannot attach it anywhere but the userspace. Messing with the userspace can be fun, but it is **not recommended** as you risk messing your dash up if you don't know what you're doing.


Collapse **Component image**

[File:InteractiveCameraControlComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=InteractiveCameraControlComponent.png "File:InteractiveCameraControlComponent.png") **Interactive Camera Control** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

See [Camera](https://wiki.resonite.com/Camera "Camera").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `_canvas` | **[Canvas](https://wiki.resonite.com/Component:Canvas "Component:Canvas")** | The canvas being used to show settings. |
| `_panel` | **[LegacyPanel](https://wiki.resonite.com/Component:LegacyPanel "Component:LegacyPanel")** | The legacy panel being used as a base to interact with the settings. |
| `FieldOfView` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The field of view for the camera. The default is `60`. |
| `AnglePosition` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The rotation around the subject. The default is `0.00`. |
| `Distance` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The distance from the camera and the subject. The default is `1.50`. |
| `HeightOffset` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The height for this camera to be at. The default is `0`. |
| `FirstPersonPitch` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Adjust the up and down angle of the camera when the camera is in `Smooth POV` mode. The default is `5.00`. |
| `FirstPersonRoll` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Adjust the rotation of the camera when the camera is in `Smooth POV` mode. The default is `0.00`. |
| `FirstPersonOffset` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Adjust the forward offset of the camera when the camera is in `Smooth POV` mode. The default is `0.02`. |
| `FramingViewportPosition` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | How to shift the camera framing like an offset. |
| `Mirror` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Mirrors the camera view. |
| `GroupDetectionRadius` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | This is the range to include users into a group photo and to have the camera focus all of them as the subject. |
| `GroupLeaveBoundary` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | This is the far range to exclude other users from the group range. |
| `PositionSmoothSpeed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How fast or slow the camera position movement should be smoothed. |
| `AngleSmoothSpeed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The smoothness of how fast this camera turns and rotates to adjust for movement, to focus towards the subject. |
| `FramingSmoothSpeed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | This is how fast the camera will move in frame towards the subject. |
| `InterpolateBetweenAnchors` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | This allows the camera to smoothly go between anchor positions and rotations. If this is off, the camera will instantly go to the anchor instead of being smooth. |
| `AnchorInterpolationSpeed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How fast to move between anchors. |
| `AnchorLinearInterpolation` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the camera should move between anchors in a linear speed fashion. |
| `Mode` | **[CameraPositioningMode](https://wiki.resonite.com/Type:CameraPositioningMode "Type:CameraPositioningMode")** | How the camera should position itself. |
| `FramingTargetOverride` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | Frame only the user with this username. |
| `CameraOperators` | _direct_ **[SyncFieldList\`1](https://wiki.resonite.com/Type:SyncFieldList%601 "Type:SyncFieldList`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | A list of people who can interact with the camera. |
| `GroupIncludeUsers` | _direct_ **[SyncFieldList\`1](https://wiki.resonite.com/Type:SyncFieldList%601 "Type:SyncFieldList`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | A list of users to force include into the target group. |
| `GroupExcludeUsers` | _direct_ **[SyncFieldList\`1](https://wiki.resonite.com/Type:SyncFieldList%601 "Type:SyncFieldList`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | A list of users to force exclude from the target group. |
| `RenderForEveryone` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | This shows the preview to any user that is looking at the preview window on the camera. |
| `AnyoneCanInteract` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | This allows any user to interact with the your camera. |
| `RenderPrivateUI` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | This shows the Camera Controls Panel to be shown in the preview and pictures. |
| `MotionBlur` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | This enables the camera to have motion blue as it moves. |
| `ScreenSpaceReflections` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | This shows screen space reflection through the preview and pictures. |
| `SpawnPhotoInWorld` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | This will spawn the photo in to the world after a picture is taken. If this is off, it will only be saved on your device. |
| `FlipPreview` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | This flips the preview window, but not for the photo being taken. This also reverses the direction for the preview window when clicking on it as well. |
| `_renderTextureProxy` | **[RenderTextureProxyProvider](https://wiki.resonite.com/Component:RenderTextureProxyProvider "Component:RenderTextureProxyProvider")** | The texture to render to. |
| `_framingReticle` | **[RectTransform](https://wiki.resonite.com/Component:RectTransform "Component:RectTransform")** | The rectangle to frame with. |
| `_mirrorMessage` | **[RectTransform](https://wiki.resonite.com/Component:RectTransform "Component:RectTransform")** | The text for the label for the mirroring button. |
| `_smoothFirstPersonButton` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | Enable/disable button for smooth first person. |
| `_thirdPersonButton` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | Enable/disable button for |
| `_groupButton` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | Enable/disable button for |
| `_worldButton` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | Enable/disable button for |
| `_manualButton` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | Enable/disable button for |
| `_mirrorButton` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | Enable/disable button for |
| `_usersButton` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | Enable/disable button for |
| `_angleIncreaseButton` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | adjust button for |
| `_angleDecreaseButton` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | adjust button for |
| `_heightIncreaseButton` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | adjust button for |
| `_heightDecreaseButton` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | adjust button for |
| `_distanceIncreaseButton` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | adjust button for |
| `_distanceDecreaseButton` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | adjust button for |
| `_resetButton` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | resets the selected options to the default value. |
| `_fovSlider` | **[Slider\`1](https://wiki.resonite.com/Component:Slider%601 "Component:Slider`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | Slider for the Field of view amount. |
| `_avoidOcclusion` | **[Checkbox](https://wiki.resonite.com/Component:Checkbox "Component:Checkbox")** | When the camera is behind a wall or anything that is collidable, it will zoom the view in front of it to focus on the subject. This will not work in manual mode. |
| `_keepInWorldSpace` | **[Checkbox](https://wiki.resonite.com/Component:Checkbox "Component:Checkbox")** | This keeps the camera in world space. |
| `_movementWobble` | **[Checkbox](https://wiki.resonite.com/Component:Checkbox "Component:Checkbox")** | This makes the camera have gradual movement in different positions around the subject. This only works with Third Person or Group modes. |
| `_aimInFrontOfHead` | **[Checkbox](https://wiki.resonite.com/Component:Checkbox "Component:Checkbox")** | This aims the camera view more towards the user's head, specifically a few inches/centimeters in front of the head proxy's forward direction. This only works for the Third Person, Group, and World modes. |
| `_forceEyesOnCamera` | **[Checkbox](https://wiki.resonite.com/Component:Checkbox "Component:Checkbox")** | This makes the user's avatar's eyes lock on to the camera position. |
| `_hideCamera` | **[Checkbox](https://wiki.resonite.com/Component:Checkbox "Component:Checkbox")** | This hides the camera visual, but will still track the subject or stay in place as before with manual mode or with camera anchors. |
| `_hideBadge` | **[Checkbox](https://wiki.resonite.com/Component:Checkbox "Component:Checkbox")** | This hides the user's badges (including the nameplate) from the camera preview and any pictures taken. |
| `_hideLasers` | **[Checkbox](https://wiki.resonite.com/Component:Checkbox "Component:Checkbox")** | This hides the user's lasers from the camera preview and any pictures taken. |
| `_showFrustum` | **[Checkbox](https://wiki.resonite.com/Component:Checkbox "Component:Checkbox")** | This shows where the camera is aimed and focused at in 3D space. |
| `_timer` | **[Checkbox](https://wiki.resonite.com/Component:Checkbox "Component:Checkbox")** | Sets up the camera to have a timer when the photo button is pressed. The timer can be set to have a preset amount of time or a custom time, found on the back of the camera itself. |
| `_forceLive` | **[Checkbox](https://wiki.resonite.com/Component:Checkbox "Component:Checkbox")** | Shows the live badge to let other user's know that you are live and streaming to somewhere external from Resonite. |
| `_audioFromCameraViewpoint` | **[Checkbox](https://wiki.resonite.com/Component:Checkbox "Component:Checkbox")** | This moves your audio listeners (your audio output or ears) to where the camera is, overriding thier position to take in audio from. This can be checked for using the [local output category](https://wiki.resonite.com/Category:ProtoFlux:Users:LocalOutput "Category:ProtoFlux:Users:LocalOutput") in [ProtoFlux](https://wiki.resonite.com/ProtoFlux "ProtoFlux"). |
| `_userControl` | **[InteractiveCameraUserControl](https://wiki.resonite.com/Component:InteractiveCameraUserControl "Component:InteractiveCameraUserControl")** | see [Interactive Camera User Control](https://wiki.resonite.com/Component:InteractiveCameraUserControl "Component:InteractiveCameraUserControl"). |
| `_settingsDialog` | **[InteractiveCameraControlSettings](https://wiki.resonite.com/Component:InteractiveCameraControlSettings "Component:InteractiveCameraControlSettings")** | see [Interactive Camera Control Settings](https://wiki.resonite.com/Component:InteractiveCameraControlSettings "Component:InteractiveCameraControlSettings"). |
| `_positioningDialog` | **[InteractiveCameraControlPositioning](https://wiki.resonite.com/Component:InteractiveCameraControlPositioning "Component:InteractiveCameraControlPositioning")** | see [Interactive Camera Control Positioning](https://wiki.resonite.com/Component:InteractiveCameraControlPositioning "Component:InteractiveCameraControlPositioning"). |
| `_anchorsDialog` | **[InteractiveCameraControlAnchors](https://wiki.resonite.com/Component:InteractiveCameraControlAnchors "Component:InteractiveCameraControlAnchors")** | see [Interactive Camera Control Anchors](https://wiki.resonite.com/Component:InteractiveCameraControlAnchors "Component:InteractiveCameraControlAnchors"). |
| `_OBS_Dialog` | **[InteractiveCameraOBS](https://wiki.resonite.com/Component:InteractiveCameraOBS "Component:InteractiveCameraOBS")** | see [Interactive Camera OBS](https://wiki.resonite.com/Component:InteractiveCameraOBS "Component:InteractiveCameraOBS"). |
| `_twitchDialog` | **[TwitchChatDialog](https://wiki.resonite.com/Component:TwitchChatDialog "Component:TwitchChatDialog")** | see [Twitch Chat Dialog](https://wiki.resonite.com/Component:TwitchChatDialog "Component:TwitchChatDialog"). |
| `_settingsButton` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | opens the settings for the camera. |
| `_positioningButton` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | Allows for changing the positioning |
| `_anchorsButton` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | Allows for changing the anchor points. |
| `_OBS_Button` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | Allows for showing and changing the OBS settings. |
| `_twitchButton` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | Allows for showing and changing the Twitch settings. |
| `_previewMaterial` | **[UI\_UnlitMaterial](https://wiki.resonite.com/Component:UI_UnlitMaterial "Component:UI UnlitMaterial")** | Shows the camera preview. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| ``OnClose:Action`1<LegacyPanel>`` | **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") < [LegacyPanel](https://wiki.resonite.com/Component:LegacyPanel "Component:LegacyPanel") >** | ✓ | Handles the closing of this panel. |
| `OnCameraControlReset:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | A setting changing handler for the panel. |
| `OnPreviewImagePress:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | A setting changing handler for the panel. |
| `OnSmoothFirstPerson:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | A setting changing handler for the panel. |
| `OnThirdPerson:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | A setting changing handler for the panel. |
| `OnGroup:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | A setting changing handler for the panel. |
| `OnWorld:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | A setting changing handler for the panel. |
| `OnManual:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | A setting changing handler for the panel. |
| `OnMirror:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | A setting changing handler for the panel. |
| `OnPhoto:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | A setting changing handler for the panel. |
| `On360Photo:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | A setting changing handler for the panel. |
| `OnUsers:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | A setting changing handler for the panel. |
| `OnCreateCameraAnchor:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | A setting changing handler for the panel. |
| `OnSettings:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | A setting changing handler for the panel. |
| `OnPositioning:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | A setting changing handler for the panel. |
| `OnAnchors:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | A setting changing handler for the panel. |
| `OnOBS:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | A setting changing handler for the panel. |
| `OnTwitch:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | A setting changing handler for the panel. |
| ``OnTwitchPin:Action`1<LegacyPanel.TitleButton>`` | **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") < [LegacyPanel.TitleButton](https://wiki.resonite.com/Component:LegacyPanel#TitleButton "Component:LegacyPanel") >** | ✓ | A setting changing handler for the panel. |

Triggers
Collapse

## Usage

See [Camera](https://wiki.resonite.com/Camera "Camera").

## Examples

See [Camera](https://wiki.resonite.com/Camera "Camera").

## See Also

- [Camera](https://wiki.resonite.com/Camera "Camera")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:InteractiveCameraControl&oldid=98930](https://wiki.resonite.com/index.php?title=Component:InteractiveCameraControl&oldid=98930)"

Contents