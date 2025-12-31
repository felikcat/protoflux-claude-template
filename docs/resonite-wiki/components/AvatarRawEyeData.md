# Component:AvatarRawEyeData

> Source: https://wiki.resonite.com/Component:AvatarRawEyeData

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:AvatarRawEyeData&diff=97396) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/a/a0/AvatarRawEyeDataComponent.png/510px-AvatarRawEyeDataComponent.png)](https://wiki.resonite.com/File:AvatarRawEyeDataComponent.png) **Avatar Raw Eye Data** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **AvatarRawEyeData** component provides the eye tracking data on a particular User. This component links to a user upon being part of an Avatar that a user equips.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `LeftEye` | _direct_ **[AvatarRawEyeData.EyeData](https://wiki.resonite.com/Component:AvatarRawEyeData#EyeData)** | Data about the left eye from the user's eye tracking device |
| `RightEye` | _direct_ **[AvatarRawEyeData.EyeData](https://wiki.resonite.com/Component:AvatarRawEyeData#EyeData)** | Data about the right eye from the user's eye tracking device |
| `CombinedEye` | _direct_ **[AvatarRawEyeData.EyeData](https://wiki.resonite.com/Component:AvatarRawEyeData#EyeData)** | Data about combined eye Data from the user's tracking device |
| `ConvergenceDistance` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The User's eye tracking convergence distance data |
| `Timestamp` | **[Double](https://wiki.resonite.com/Type:Double "Type:Double")** | The timestamp value gotten directly from the eye tracking device. |
| `_activeUser` | **[User](https://wiki.resonite.com/Type:User "Type:User")** | The user that the component is reading eye tracking data from. |

Fields
Collapse

## EyeData

| Name | Type | Description |
| --- | --- | --- |
| `IsTracking` | **[bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the device is tracking this eye. |
| `Origin` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The position of the eyeball. |
| `Direction` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | the direction the eye is looking |
| `PupilDiameter` | **[float](https://wiki.resonite.com/Type:Float "Type:Float")** | The diameter of the eyes in mm |
| `Openness` | **[float](https://wiki.resonite.com/Type:Float "Type:Float")** | Whether the eyes are open or closed. |
| `Widen` | **[float](https://wiki.resonite.com/Type:Float "Type:Float")** | how wide the eyes are in surprise |
| `Squeeze` | **[float](https://wiki.resonite.com/Type:Float "Type:Float")** | how much the eyes are squinting |
| `Frown` | **[float](https://wiki.resonite.com/Type:Float "Type:Float")** | how much the eyes are affected by the face stretching into a frown |
| `InnerBrowVertical` | **[float](https://wiki.resonite.com/Type:Float "Type:Float")** | The vertical movement of the inner edge of the eyebrow |
| `OuterBrowVertical` | **[float](https://wiki.resonite.com/Type:Float "Type:Float")** | The vertical movement of the outer edge of the eyebrow |

Fields

## Usage

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AvatarRawEyeData&oldid=97396](https://wiki.resonite.com/index.php?title=Component:AvatarRawEyeData&oldid=97396)"

Contents