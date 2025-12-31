# Component:FingerSplayModifier

> Source: https://wiki.resonite.com/Component:FingerSplayModifier

Collapse **Component image**

[File:FingerSplayModifierComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=FingerSplayModifierComponent.png "File:FingerSplayModifierComponent.png") **Finger Splay Modifier** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **FingerSplayModifier** takes data from a `Source`, adding splay data to a copy of that data. The resulting data becomes the pose source data of this component. This component in itself is a [IFingerPoseSourceComponent](https://wiki.resonite.com/Type:IFingerPoseSourceComponent "Type:IFingerPoseSourceComponent").

For more information on finger pose sources, please see [Finger Posing System](https://wiki.resonite.com/Finger_Posing_System "Finger Posing System").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Source` | **[IFingerPoseSourceComponent](https://wiki.resonite.com/Type:IFingerPoseSourceComponent "Type:IFingerPoseSourceComponent")** | The source data to copy to this component's Finger pose source data. |
| `LeftSplayMagnitude` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much splay data to the left hand to add to the data copied data from `Source` during copying. |
| `RightSplayMagnitude` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much splay data on the right hand to add to the data copied data from `Source` during copying. |

Fields
Collapse

## Usage

Used as a way of modifying Finger pose data to splay the fingers, and itself be used as new finger pose data.

## Examples

[video from Frooxius (works near end of the video)](https://youtu.be/DXmQOtOTSrw)

## See Also

- [Finger Posing System](https://wiki.resonite.com/Finger_Posing_System "Finger Posing System")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:FingerSplayModifier&oldid=94727](https://wiki.resonite.com/index.php?title=Component:FingerSplayModifier&oldid=94727)"

Contents