# Component:FingerPoseModifier

> Source: https://wiki.resonite.com/Component:FingerPoseModifier

Collapse **Component image**

[File:FingerPoseModifierComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=FingerPoseModifierComponent.png "File:FingerPoseModifierComponent.png") **Finger Pose Modifier** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **FingerPoseModifier** component takes a `Source` and makes a copy of the finger pose data from it. It then modifies the copied data before making it the finger pose data of this component. This component in itself is a [IFingerPoseSourceComponent](https://wiki.resonite.com/Type:IFingerPoseSourceComponent "Type:IFingerPoseSourceComponent").

For more information on finger pose sources, please see [Finger Posing System](https://wiki.resonite.com/Finger_Posing_System "Finger Posing System").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Source` | **[IFingerPoseSourceComponent](https://wiki.resonite.com/Type:IFingerPoseSourceComponent "Type:IFingerPoseSourceComponent")** | The component to take finger pose data from and make a copy to modify and make this component's finger pose data. |
| `LeftOffsets` | _direct_ **[FingerPoseModifier.FingerOffsets](https://wiki.resonite.com/Component:FingerPoseModifier#FingerOffsets)** | How to modify the left finger pose data before making it this component's finger pose data. |
| `RightOffsets` | _direct_ **[FingerPoseModifier.FingerOffsets](https://wiki.resonite.com/Component:FingerPoseModifier#FingerOffsets)** | How to modify the right finger pose data before making it this component's finger pose data. |

Fields
Collapse

## FingerOffsets

| Name | Type | Description |
| --- | --- | --- |
| `ThumbCurlOffset` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much curl to add to the thumb. |
| `IndexCurlOffset` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much curl to add to the index finger. |
| `MiddleCurlOffset` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much curl to add to the middle finger. |
| `RingCurlOffset` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much curl to add to the ring finger. |
| `PinkyCurlOffset` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much curl to add to the pinky finger. |
| `ThumbSplayOffset` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much splaying to add to the thumb. |
| `IndexSplayOffset` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much splaying to add to the index finger. |
| `MiddleSplayOffset` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much splaying to add to the middle finger. |
| `RingSplayOffset` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much splaying to add to the ring finger. |
| `PinkySplayOffset` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much splaying to add to the pinky finger. |

Fields

## Usage

Provide the component with data from another [IFingerPoseSourceComponent](https://wiki.resonite.com/Type:IFingerPoseSourceComponent "Type:IFingerPoseSourceComponent") to add extra offsets onto. This component can be used as a [IFingerPoseSourceComponent](https://wiki.resonite.com/Type:IFingerPoseSourceComponent "Type:IFingerPoseSourceComponent") for other components.

## Examples

[Frooxius devlog video on this component](https://youtu.be/PG4qnZluan4)

## See Also

- [Finger Posing System](https://wiki.resonite.com/Finger_Posing_System "Finger Posing System")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:FingerPoseModifier&oldid=97506](https://wiki.resonite.com/index.php?title=Component:FingerPoseModifier&oldid=97506)"

Contents