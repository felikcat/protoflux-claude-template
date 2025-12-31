# Component:LegacyAudioPlayer

> Source: https://wiki.resonite.com/Component:LegacyAudioPlayer

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This article describes a feature marked as legacy—this usually means there's a newer, better alternative. Legacy features might not be removed but they will not be updated, and the [team](https://wiki.resonite.com/Resonite_Team "Resonite Team") will not provide any support for them.


Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/4/47/LegacyAudioPlayerComponent.png/510px-LegacyAudioPlayerComponent.png)](https://wiki.resonite.com/File:LegacyAudioPlayerComponent.png) **Legacy Audio Player** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **LegacyAudioPlayer** component is a leftover Component from content migrated from other platforms. It should not be used, and should be replaced whenever possible.

For a replacement see [Audio Player](https://wiki.resonite.com/Audio_Player "Audio Player").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `AudioClip` | **[AudioClip](https://wiki.resonite.com/Type:AudioClip "Type:AudioClip")** | The audio clip for this audio player. |
| `_clipPlayer` | **[AudioClipPlayer](https://wiki.resonite.com/Component:AudioClipPlayer "Component:AudioClipPlayer")** | The audio clip player that will play the audio clip. |
| `_audioOutput` | **[AudioOutput](https://wiki.resonite.com/Component:AudioOutput "Component:AudioOutput")** | The audio output for the audio clip. |
| `_waveformMaterial` | **[UnlitMaterial](https://wiki.resonite.com/Component:UnlitMaterial "Component:UnlitMaterial")** | The material that is used on the ring visual. |
| `_playbackMaterial` | **[UnlitMaterial](https://wiki.resonite.com/Component:UnlitMaterial "Component:UnlitMaterial")** | The material that is used for the playback visual. |
| `_waveformRingMesh` | **[RingMesh](https://wiki.resonite.com/Component:RingMesh "Component:RingMesh")** | The mesh used for the waveform ring visual. |
| `_playbackRingMesh` | **[RingMesh](https://wiki.resonite.com/Component:RingMesh "Component:RingMesh")** | The mesh used for the playback ring visual. |
| `_playbackRingArc` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The field to drive to make the visual for the playback ring. |
| `_volumeRingArc` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The field to drive to make the visual for the audio arc. |
| `_playbackTimeText` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | The field to drive for the playback time text. |
| `_clipLengthTimeText` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | The field to drive for the audio clip length text. |
| `_iconTextureURL` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Uri](https://wiki.resonite.com/Type:Uri "Type:Uri")** | The field to drive with the icon texture URI. |
| `_stopItem` | **[LegacySegmentCircleMenuController.Item](https://wiki.resonite.com/Component:LegacySegmentCircleMenuController#Item "Component:LegacySegmentCircleMenuController")** | The item that can be clicked to stop playback. |
| `_loopItem` | **[LegacySegmentCircleMenuController.Item](https://wiki.resonite.com/Component:LegacySegmentCircleMenuController#Item "Component:LegacySegmentCircleMenuController")** | The item that can be clicked to loop playback. |
| `_spatialItem` | **[LegacySegmentCircleMenuController.Item](https://wiki.resonite.com/Component:LegacySegmentCircleMenuController#Item "Component:LegacySegmentCircleMenuController")** | The item that can be clicked to spatialize or unspatialize the audio. |
| `_loopIconURL` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Uri](https://wiki.resonite.com/Type:Uri "Type:Uri")** | The field to drive with the loop icon texture URI. |
| `_spatialIconURL` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Uri](https://wiki.resonite.com/Type:Uri "Type:Uri")** | The field to drive with the spatialize icon URI. |
| `_exportable` | **[AudioExportable](https://wiki.resonite.com/Component:AudioExportable "Component:AudioExportable")** | The audio exportable component used to handle the export behavior of this audio player. |
| `_assetProxy` | **[AssetProxy\`1](https://wiki.resonite.com/Component:AssetProxy%601 "Component:AssetProxy`1") < [AudioClip](https://wiki.resonite.com/Type:AudioClip "Type:AudioClip") >** | The asset proxy used to handle dropping this audio player into fields that accept audio clips. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| ``StopPressed:Action`1<LegacySegmentCircleMenuController.Item>`` | **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") < [LegacySegmentCircleMenuController.Item](https://wiki.resonite.com/Component:LegacySegmentCircleMenuController#Item "Component:LegacySegmentCircleMenuController") >** | ✓ | A sync delegate to call when the stop button is pressed. |
| ``LoopToggle:Action`1<LegacySegmentCircleMenuController.Item>`` | **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") < [LegacySegmentCircleMenuController.Item](https://wiki.resonite.com/Component:LegacySegmentCircleMenuController#Item "Component:LegacySegmentCircleMenuController") >** | ✓ | A sync delegate to call when the loop button is pressed. |
| ``SpatialToggle:Action`1<LegacySegmentCircleMenuController.Item>`` | **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") < [LegacySegmentCircleMenuController.Item](https://wiki.resonite.com/Component:LegacySegmentCircleMenuController#Item "Component:LegacySegmentCircleMenuController") >** | ✓ | A sync delegate to call when the spatialize button is pressed. |

Triggers
Collapse

## Usage

Not to be used.

## Examples

Old content migrated from other platforms.

## See Also

- [Audio Player](https://wiki.resonite.com/Audio_Player "Audio Player")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:LegacyAudioPlayer&oldid=99008](https://wiki.resonite.com/index.php?title=Component:LegacyAudioPlayer&oldid=99008)"

Contents