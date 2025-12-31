# Component:PhotoCaptureManager

> Source: https://wiki.resonite.com/Component:PhotoCaptureManager

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/2/2c/PhotoCaptureManagerComponent.png/510px-PhotoCaptureManagerComponent.png)](https://wiki.resonite.com/File:PhotoCaptureManagerComponent.png) **Photo Capture Manager** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **PhotoCaptureManager** component is used to manage the finger photo capture ability for users and what settings to use for it.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `FingerGestureEnabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the finger photo gesture can be used or not. |
| `MinDistance` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The distance from the view to use for minimum FOV point. |
| `MaxDistance` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The distance from the view to use for maximum FOV point. |
| `MinFOV` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The minimum FOV that can be achieved by moving the finger photo closer to the viewpoint. |
| `MaxFOV` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The maximum FOV that can be achieved by moving the finger photo further from the viewpoint. |
| `PreviewResolution` | **[Int2](https://wiki.resonite.com/Type:Int2 "Type:Int2")** | The resolution of the texture shown on the preview graphic. |
| `NormalResolution` | **[Int2](https://wiki.resonite.com/Type:Int2 "Type:Int2")** | The resolution of the picture taken normally. |
| `TimerResolution` | **[Int2](https://wiki.resonite.com/Type:Int2 "Type:Int2")** | The resolution of the picture taken via camera. |
| `CaptureStereo` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the finger photo should capture a 3D photo. |
| `StereoSeparation` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to separate the L and R "eye" positions for the camera capture. |
| `TimerSeconds` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How many seconds the finger photo timer should be. |
| `HideAllNameplates` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to hide all nameplates for taking the photo. |
| `EncodeFormat` | **[PhotoEncodeFormat](https://wiki.resonite.com/Type:PhotoEncodeFormat "Type:PhotoEncodeFormat")** | What format to encode the resulting picture in. |
| `DebugGesture` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to debug the user's gesture angles/position for achieving a valid finger photo gesture position. |
| `_timerStart` | _direct_ **[SyncTime](https://wiki.resonite.com/Type:SyncTime "Type:SyncTime")** | What time the last timer started at. |
| `_timerActive` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the timer is currently going or not. |
| `_originalParent` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The original parent of this manager. |
| `_originalPosition` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The original position of this manager. |
| `_originalRotation` | **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The original rotation of this manager. |
| `_originalScale` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The original scale of this manager. |
| `_root` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The root of this entire finger photo manager. |
| `_previewRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot that is the root of the preview graphic. |
| `_renderTex` | **[RenderTextureProvider](https://wiki.resonite.com/Component:RenderTextureProvider "Component:RenderTextureProvider")** | The texture being used for the preview render graphic. |
| `_quad` | **[QuadMesh](https://wiki.resonite.com/Component:QuadMesh "Component:QuadMesh")** | The quad to render the preview with. |
| `_frame` | **[FrameMesh](https://wiki.resonite.com/Component:FrameMesh "Component:FrameMesh")** | The frame mesh being used for the preview graphic. |
| `_cameraRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot being used for the camera's transforms. |
| `_cameraPos` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The position field of the camera. |
| `_cameraRot` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The rotation field of the camera. |
| `_camera` | **[Camera](https://wiki.resonite.com/Component:Camera "Component:Camera")** | The camera component reference itself. |
| `_frameMaterial` | **[UnlitMaterial](https://wiki.resonite.com/Component:UnlitMaterial "Component:UnlitMaterial")** | The material being used for the frame visual for the preview graphic. |
| `_timerTextRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The root slot of the visual being used for the timer text. |
| `_timerText` | **[TextRenderer](https://wiki.resonite.com/Component:TextRenderer "Component:TextRenderer")** | The component being used to display the timer text. |
| `_shutterClip` | **[AudioClip](https://wiki.resonite.com/Type:AudioClip "Type:AudioClip")** | The audio to play when a photo is taken. |
| `_timerStartClip` | **[AudioClip](https://wiki.resonite.com/Type:AudioClip "Type:AudioClip")** | The audio to play when the timer starts. |
| `_timerCountdownSlowPlayer` | **[AudioClipPlayer](https://wiki.resonite.com/Component:AudioClipPlayer "Component:AudioClipPlayer")** | The audio to play when the timer has plenty of time left. |
| `_timerCountdownFastPlayer` | **[AudioClipPlayer](https://wiki.resonite.com/Component:AudioClipPlayer "Component:AudioClipPlayer")** | The audio to play when the timer is close to being finished. |
| `_timerCountdownSlowOutput` | **[AudioOutput](https://wiki.resonite.com/Component:AudioOutput "Component:AudioOutput")** | The audio output component outputting the timer has plenty of time sound. |
| `_timerCountdownFastOutput` | **[AudioOutput](https://wiki.resonite.com/Component:AudioOutput "Component:AudioOutput")** | The audio output component outputting the timer is close to being done sound. |
| `_timerRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The root slot of the entire timer visual and mechanism. |

Fields
Collapse

## Usage

Not used directly by the user. auto generated.

## Examples

Used to handle finger photo taking for users.

## See Also

- [Component:PhotoCaptureSettings](https://wiki.resonite.com/Component:PhotoCaptureSettings "Component:PhotoCaptureSettings")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:PhotoCaptureManager&oldid=106248](https://wiki.resonite.com/index.php?title=Component:PhotoCaptureManager&oldid=106248)"

Contents