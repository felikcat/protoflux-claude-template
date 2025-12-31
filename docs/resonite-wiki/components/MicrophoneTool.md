# Component:MicrophoneTool

> Source: https://wiki.resonite.com/Component:MicrophoneTool

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/0/0a/MicrophoneToolComponent.png/510px-MicrophoneToolComponent.png)](https://wiki.resonite.com/File:MicrophoneToolComponent.png) **Microphone Tool** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

See [Microphone](https://wiki.resonite.com/Microphone "Microphone").

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `_equipLink` | _direct_ **[LinkTarget\`1](https://wiki.resonite.com/index.php?title=Type:LinkTarget%601&action=edit&redlink=1 "Type:LinkTarget`1 (page does not exist)") < [ITool](https://wiki.resonite.com/Type:ITool "Type:ITool") >** | This is Internal, and is used by the engine to retrieve the component this field is a part of. It cannot be assigned to. |
| `TipReference` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot to use as the tool's tip, instead of the component's slot. |
| `BlockGripEquip` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to prevent legacy double grip equipping from equipping this tooltip. |
| `BlockRemoteEquip` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to prevent equipping by clicking via laser |
| `EquipName` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The name of the tool in the context menu when equipping via context menu. |
| `_overrideActiveTool` | **[InteractionHandler](https://wiki.resonite.com/Component:InteractionHandler "Component:InteractionHandler")** | The interaction handler to use instead of this tool as an interaction handler. |
| `_gripPosesGenerated` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the [Grip Pose Reference](https://wiki.resonite.com/Component:GripPoseReference "Component:GripPoseReference") components and slots have been generated for this tool. |
| `Format` | **[MicrophoneTool.RecordFormat](https://wiki.resonite.com/Component:MicrophoneTool#RecordFormat)** | The type of audio file to make. |
| `Quality` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The quality of the resulting audio clip file. |
| `Mode` | **[MicrophoneTool.RecordMode](https://wiki.resonite.com/Component:MicrophoneTool#RecordMode)** | Whether the user has to hold or it's a toggle. |
| `Source` | **[MicrophoneTool.DataSource](https://wiki.resonite.com/Component:MicrophoneTool#DataSource)** | The way to record the audio. |
| `RecordingUser` | **[User](https://wiki.resonite.com/Type:User "Type:User")** | The user that is currently recording using the Tool. |
| `RecordingStartTime` | _direct_ **[SyncTime](https://wiki.resonite.com/Type:SyncTime "Type:SyncTime")** | The time that the user started recording in world time. |
| `IsRecording` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the tool is currently being used to record. |

Fields
Collapse

## RecordFormat

| Name | Value | Description |
| --- | --- | --- |
| `OGG_Vorbis` | 0 | Directional audio with a left and right position. |
| `WAV` | 1 | Windows audio format |
| `FLAC` | 2 | Zero compression high quality format. |

Values

## RecordMode

| Name | Value | Description |
| --- | --- | --- |
| `Hold` | 0 | The user has to hold Primary down to record |
| `Toggle` | 1 | The user has to press Primary to start recording and then press it again to stop recording. |

Values

## DataSource

| Name | Value | Description |
| --- | --- | --- |
| `RAW` | 0 | Raw audio, no normalization |
| `Normalized` | 1 | Normalized audio, makes audio recording consistent between mic gains. |

Values

## Usage

See [Microphone](https://wiki.resonite.com/Microphone "Microphone").

## Examples

See [Microphone](https://wiki.resonite.com/Microphone "Microphone").

## See Also

- [Microphone](https://wiki.resonite.com/Microphone "Microphone")
- [Tools](https://wiki.resonite.com/Tools "Tools")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:MicrophoneTool&oldid=97624](https://wiki.resonite.com/index.php?title=Component:MicrophoneTool&oldid=97624)"

Contents