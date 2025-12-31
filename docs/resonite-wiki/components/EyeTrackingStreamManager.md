# Component:EyeTrackingStreamManager

> Source: https://wiki.resonite.com/Component:EyeTrackingStreamManager

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:EyeTrackingStreamManager&diff=97487) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/b/b2/EyeTrackingStreamManagerComponent.png/510px-EyeTrackingStreamManagerComponent.png)](https://wiki.resonite.com/File:EyeTrackingStreamManagerComponent.png) **EyeTrackingStreamManager** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **EyeTrackingStreamManager** component uses streaming data from the [ValueStream](https://wiki.resonite.com/index.php?title=Type:ValueStream%601&action=edit&redlink=1 "Type:ValueStream`1 (page does not exist)") data type (seen in the [user Inspector](https://wiki.resonite.com/User_Inspector "User Inspector")) to control the left and right eyes on a [user's](https://wiki.resonite.com/User "User") [avatar](https://wiki.resonite.com/Avatar "Avatar").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `User` | **[User](https://wiki.resonite.com/Type:User "Type:User")** | The focused user to get streaming data from. |
| `ConvergenceDistance` | **[ValueStream\`1](https://wiki.resonite.com/index.php?title=Type:ValueStream%601&action=edit&redlink=1 "Type:ValueStream`1 (page does not exist)") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | The eye distance data from the headset. |
| `IsEyeTrackingActive` | **[ValueStream\`1](https://wiki.resonite.com/index.php?title=Type:ValueStream%601&action=edit&redlink=1 "Type:ValueStream`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >** | Returns true if the eyes are being tracked from the headset. |
| `LeftEyeStreams` | _direct_ **[EyeTrackingStreamManager.EyeStreams](https://wiki.resonite.com/Component:EyeTrackingStreamManager#EyeStreams)** | A set of fields for the left eye. |
| `RightEyeStreams` | _direct_ **[EyeTrackingStreamManager.EyeStreams](https://wiki.resonite.com/Component:EyeTrackingStreamManager#EyeStreams)** | A set of fields for the right eye. |

Fields
Collapse

## EyeStreams

| Name | Type | Description |
| --- | --- | --- |
| `IsTracking` | **[ValueStream\`1](https://wiki.resonite.com/index.php?title=Type:ValueStream%601&action=edit&redlink=1 "Type:ValueStream`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >** | Returns if this eye is tracking. |
| `Position` | **[ValueStream\`1](https://wiki.resonite.com/index.php?title=Type:ValueStream%601&action=edit&redlink=1 "Type:ValueStream`1 (page does not exist)") < [Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3") >** | Returns the position of the eye. |
| `Direction` | **[ValueStream\`1](https://wiki.resonite.com/index.php?title=Type:ValueStream%601&action=edit&redlink=1 "Type:ValueStream`1 (page does not exist)") < [Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3") >** | Returns where the eye is looking. |
| `Openness` | **[ValueStream\`1](https://wiki.resonite.com/index.php?title=Type:ValueStream%601&action=edit&redlink=1 "Type:ValueStream`1 (page does not exist)") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | Returns how open the eye is. |
| `Widen` | **[ValueStream\`1](https://wiki.resonite.com/index.php?title=Type:ValueStream%601&action=edit&redlink=1 "Type:ValueStream`1 (page does not exist)") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | Returns how wide the eye is. |
| `Squeeze` | **[ValueStream\`1](https://wiki.resonite.com/index.php?title=Type:ValueStream%601&action=edit&redlink=1 "Type:ValueStream`1 (page does not exist)") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | Returns how squeezed the eye is. |
| `Frown` | **[ValueStream\`1](https://wiki.resonite.com/index.php?title=Type:ValueStream%601&action=edit&redlink=1 "Type:ValueStream`1 (page does not exist)") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | Returns if the eye is frowning. |
| `InnerBrowVertical` | **[ValueStream\`1](https://wiki.resonite.com/index.php?title=Type:ValueStream%601&action=edit&redlink=1 "Type:ValueStream`1 (page does not exist)") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | Returns the inner brow data. |
| `OuterBrowVertical` | **[ValueStream\`1](https://wiki.resonite.com/index.php?title=Type:ValueStream%601&action=edit&redlink=1 "Type:ValueStream`1 (page does not exist)") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | Returns the outer brow data. |
| `PupilDiameter` | **[ValueStream\`1](https://wiki.resonite.com/index.php?title=Type:ValueStream%601&action=edit&redlink=1 "Type:ValueStream`1 (page does not exist)") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | Returns the pupil diameter. |

Fields

## Usage

Used for [Eye Tracking](https://wiki.resonite.com/index.php?title=Eye_Tracking&action=edit&redlink=1 "Eye Tracking (page does not exist)").

## Examples

## See Also

- [Component:EyeLinearDriver](https://wiki.resonite.com/Component:EyeLinearDriver "Component:EyeLinearDriver")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:EyeTrackingStreamManager&oldid=97487](https://wiki.resonite.com/index.php?title=Component:EyeTrackingStreamManager&oldid=97487)"

Contents