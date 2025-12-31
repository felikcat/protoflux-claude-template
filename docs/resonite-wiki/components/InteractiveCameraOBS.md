# Component:InteractiveCameraOBS

> Source: https://wiki.resonite.com/Component:InteractiveCameraOBS

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/3/36/InteractiveCameraOBSComponent.png/510px-InteractiveCameraOBSComponent.png)](https://wiki.resonite.com/File:InteractiveCameraOBSComponent.png) **Interactive Camera OBS** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

See [Camera](https://wiki.resonite.com/Camera "Camera").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `_canvas` | **[Canvas](https://wiki.resonite.com/Component:Canvas "Component:Canvas")** | The canvas being used to show settings. |
| `_panel` | **[LegacyPanel](https://wiki.resonite.com/Component:LegacyPanel "Component:LegacyPanel")** | The legacy panel being used as a base to interact with the settings. |
| `_currentPanel` | **[RectTransform](https://wiki.resonite.com/Component:RectTransform "Component:RectTransform")** | the rectangle transform of the currently viewed panel. |
| `_container` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot to store UI elements. |
| `CameraControl` | **[InteractiveCameraControl](https://wiki.resonite.com/Component:InteractiveCameraControl "Component:InteractiveCameraControl")** | see [Interactive Camera Control](https://wiki.resonite.com/Component:InteractiveCameraControl "Component:InteractiveCameraControl"). |
| `_connectAddress` | **[TextField](https://wiki.resonite.com/Component:TextField "Component:TextField")** | The field to read an OBS websocket connect address from. |
| `_connectPassword` | **[TextField](https://wiki.resonite.com/Component:TextField "Component:TextField")** | The field to read an OBS websocket connect password from. |
| `_status` | **[Text](https://wiki.resonite.com/Component:Text "Component:Text")** | The current status of the OBS connection. |
| `_active` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the connection is active |
| `_streamTime` | **[Text](https://wiki.resonite.com/Component:Text "Component:Text")** | The text to fill with how long the user has been streaming. |
| `_bytesPerSec` | **[Text](https://wiki.resonite.com/Component:Text "Component:Text")** | The text to fill with how many bytes per second the user is streaming. |
| `_fps` | **[Text](https://wiki.resonite.com/Component:Text "Component:Text")** | The text to fill with how many frames per second the user is streaming. |
| `_droppedFrames` | **[Text](https://wiki.resonite.com/Component:Text "Component:Text")** | The text to fill with how many dropped frames the user has had streaming. |
| `_streamButton` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | the button that will start the streaming process to OBS. |
| `_recordButton` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | the button to start recording using OBS. |
| `_recordingStarted` | _direct_ **[SyncTime](https://wiki.resonite.com/Type:SyncTime "Type:SyncTime")** | The field to fill with when the user started recording. |
| `_launchOBSbutton` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | the button to boot OBS for the user when pressed. |
| `_autoMirror` | **[Checkbox](https://wiki.resonite.com/Component:Checkbox "Component:Checkbox")** | The button to enable the auto mirror option. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `OnReturnToConnect:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | A setting changing handler for the panel. |
| `OnLaunchOBS:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | A setting changing handler for the panel. |
| `OnConnect:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | A setting changing handler for the panel. |
| `OnStream:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | A setting changing handler for the panel. |
| `OnRecord:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | A setting changing handler for the panel. |

Triggers
Collapse

## Usage

See [Camera](https://wiki.resonite.com/Camera "Camera").

## Examples

See [Camera](https://wiki.resonite.com/Camera "Camera").

## See Also

- [Camera](https://wiki.resonite.com/Camera "Camera")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:InteractiveCameraOBS&oldid=98932](https://wiki.resonite.com/index.php?title=Component:InteractiveCameraOBS&oldid=98932)"

Contents