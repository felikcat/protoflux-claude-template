# Component:ChildParentAudioClipPlayer

> Source: https://wiki.resonite.com/Component:ChildParentAudioClipPlayer

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/c/cd/ChildParentAudioClipPlayerComponent.png/510px-ChildParentAudioClipPlayerComponent.png)](https://wiki.resonite.com/File:ChildParentAudioClipPlayerComponent.png) **Child Parent Audio Clip Player** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ChildParentAudioClipPlayer** component plays specified audio clips when it's immediate children are added to or removed from.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `ParentUnder` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | Where to parent the slots to when playing sounds. (DON'T SET THIS TO THE SLOT THIS COMPONENT IS ON. else it will spam audio every game tick) |
| `MinDistance` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | The override for all [ClipDatas](https://wiki.resonite.com/Type:ClipData "Type:ClipData") Min Distance when they are played. |
| `MaxDistance` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | The override for all [ClipDatas](https://wiki.resonite.com/Type:ClipData "Type:ClipData") Max Distance when they are played. |
| `RolloffMode` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [AudioRolloffMode](https://wiki.resonite.com/Type:AudioRolloffMode "Type:AudioRolloffMode") >** | The override for all [ClipDatas](https://wiki.resonite.com/Type:ClipData "Type:ClipData") Rolloff Mode when they are played. |
| `PlayPointMode` | **[ChildParentAudioClipPlayer.PointMode](https://wiki.resonite.com/Component:ChildParentAudioClipPlayer#PointMode)** | Where to position audio clips when they are played. |
| `ChildLimit` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | If the immediate children count of this component's slot is above this amount, it will not play sounds. |
| `FilterTag` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | If an added or removed immediate child has a tag that matches this value, a sound will not be played. |
| `ParentedClips` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[ClipData](https://wiki.resonite.com/Type:ClipData "Type:ClipData")** | A list of audio clips to play when a slot is added to the immediate children of this component's slot. |
| `UnparentedClips` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[ClipData](https://wiki.resonite.com/Type:ClipData "Type:ClipData")** | A list of audio clips to play when a slot is removed from the immediate children of this component's slot. |

Fields
Collapse

## PointMode

| Name | Value | Description |
| --- | --- | --- |
| `ParentOrigin` | 0 | Play the audio at the global position of this component's slot. |
| `ChildOrigin` | 1 | Play the audio at the global position of the slot being added or removed. |
| `ParentBoundsCenter` | 2 | Play the audio at the global center of the bounding box of this component's slot. |
| `ChildBoundsCenter` | 3 | Play the audio at the global center of the bounding box of the slot being added or removed. |

Values

## Usage

## Examples

## See Also

- [Component:RandomAudioClipPlayer](https://wiki.resonite.com/Component:RandomAudioClipPlayer "Component:RandomAudioClipPlayer")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ChildParentAudioClipPlayer&oldid=97437](https://wiki.resonite.com/index.php?title=Component:ChildParentAudioClipPlayer&oldid=97437)"

Contents