# Component:AudioMetadata

> Source: https://wiki.resonite.com/Component:AudioMetadata

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:AudioMetadata&diff=97856) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/5/58/AudioMetadataComponent.png/510px-AudioMetadataComponent.png)](https://wiki.resonite.com/File:AudioMetadataComponent.png) **Audio Metadata** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **AudioMetadata** component provides information about an audio clip. It is automatically added to audio clips recorded with the [Microphone Tool](https://wiki.resonite.com/Component:MicrophoneTool "Component:MicrophoneTool") and stores data about when, where, and by whom the audio was recorded.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `LocationName` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | Name of the session the audio was recorded in |
| `LocationURL` | **[Uri](https://wiki.resonite.com/Type:Uri "Type:Uri")** | the URI of the world the audio was recorded in |
| `LocationHost` | _direct_ **[UserRef](https://wiki.resonite.com/Type:UserRef "Type:UserRef")** | Host of the session the audio was recorded in |
| `LocationAccessLevel` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [SessionAccessLevel](https://wiki.resonite.com/Type:SessionAccessLevel "Type:SessionAccessLevel") >** | Access level of the session the audio was recorded in |
| `LocationHiddenFromListing` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >** | Whether the session was marked as hidden when the audio was recorded. |
| `TimeTaken` | **[DateTime](https://wiki.resonite.com/Type:DateTime "Type:DateTime")** | Exact timestamp that the audio was recorded at |
| `TakenBy` | _direct_ **[UserRef](https://wiki.resonite.com/Type:UserRef "Type:UserRef")** | The user who recorded the audio |
| `TakenGlobalPosition` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | the position in global space the microphone tip was at the time of recording. |
| `TakenGlobalRotation` | **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | the rotation in global space the microphone tip was at the time of recording. |
| `TakenGlobalScale` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | the scale in global space the microphone tip was at the time of recording. |
| `AppVersion` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | Resonite version number of the recording user |
| `UserInfos` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[AssetMetadata.UserInfo](https://wiki.resonite.com/Component:AssetMetadata#UserInfo "Component:AssetMetadata")** | Users present at the time of recording |
| `__legacyPresentUsers` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[UserRef](https://wiki.resonite.com/Type:UserRef "Type:UserRef")** | legacy list of users present at the time of recording. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `SetFromCurrentWorld:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | fills in all the fields using the current session data and the local user (the user running this method) |

Triggers
Collapse

## Usage

This component is essentially a bunch of fields with semantic meaning to them. Usage of this component outside of the microphone tool is straightforward--one simply needs to write to the relevant fields the relevant data. It is common convention to place the component on the same slot that the audio clip resides.

## Examples

## See Also

- [Component:MicrophoneTool](https://wiki.resonite.com/Component:MicrophoneTool "Component:MicrophoneTool")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AudioMetadata&oldid=97856](https://wiki.resonite.com/index.php?title=Component:AudioMetadata&oldid=97856)"

Contents