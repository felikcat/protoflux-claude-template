# Component:FingerPoseLerp

> Source: https://wiki.resonite.com/Component:FingerPoseLerp

Collapse **Component image**

[File:FingerPoseLerpComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=FingerPoseLerpComponent.png "File:FingerPoseLerpComponent.png") **Finger Pose Lerp** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **FingerPoseLerp** component allows for a linear blending between two different Finger pose sources. The resulting data becomes the pose source data of this component. This component in itself is a [IFingerPoseSourceComponent](https://wiki.resonite.com/Type:IFingerPoseSourceComponent "Type:IFingerPoseSourceComponent").

For more information on finger pose sources, please see [Finger Posing System](https://wiki.resonite.com/Finger_Posing_System "Finger Posing System").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `A` | **[IFingerPoseSourceComponent](https://wiki.resonite.com/Type:IFingerPoseSourceComponent "Type:IFingerPoseSourceComponent")** | The pose to start at when interpolating. |
| `B` | **[IFingerPoseSourceComponent](https://wiki.resonite.com/Type:IFingerPoseSourceComponent "Type:IFingerPoseSourceComponent")** | The pose to end at when interpolating. |
| `Lerp` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The value to use 0<->1 when interpolating from `A`<->`B` |

Fields
Collapse

## Usage

Can be used as a way of blending two different Finger pose data sources and then be used as a new finger pose data source that is the blend of the original two sources in other components.

## Examples

[Frooxius devlog on this component](https://youtu.be/Ra3Z19QHQKg)

## See Also

- [Finger Posing System](https://wiki.resonite.com/Finger_Posing_System "Finger Posing System")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:FingerPoseLerp&oldid=94726](https://wiki.resonite.com/index.php?title=Component:FingerPoseLerp&oldid=94726)"

Contents