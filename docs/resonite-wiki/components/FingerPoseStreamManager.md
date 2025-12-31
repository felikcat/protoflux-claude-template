# Component:FingerPoseStreamManager

> Source: https://wiki.resonite.com/Component:FingerPoseStreamManager

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:FingerPoseStreamManager&diff=97343) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/3/39/FingerPoseStreamManagerComponent.png/510px-FingerPoseStreamManagerComponent.png)](https://wiki.resonite.com/File:FingerPoseStreamManagerComponent.png) **FingerPoseStreamManager** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **FingerPoseStreamManager** component uses streaming data from the [ValueStream](https://wiki.resonite.com/index.php?title=Component:ValueStream&action=edit&redlink=1 "Component:ValueStream (page does not exist)") component (seen in the [user Inspector](https://wiki.resonite.com/User_Inspector "User Inspector")) to control the left and right fingers on a [user's](https://wiki.resonite.com/User "User") [avatar](https://wiki.resonite.com/Avatar "Avatar"). This component in itself is a [IFingerPoseSourceComponent](https://wiki.resonite.com/Type:IFingerPoseSourceComponent "Type:IFingerPoseSourceComponent").

For more information on finger pose sources, please see [Finger Posing System](https://wiki.resonite.com/Finger_Posing_System "Finger Posing System").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `User` | **[User](https://wiki.resonite.com/Type:User "Type:User")** | The referenced user to get tracking data from. |
| `LeftIsTracking` | **[ValueStream\`1](https://wiki.resonite.com/index.php?title=Type:ValueStream%601&action=edit&redlink=1 "Type:ValueStream`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >** | The stream data for the left hand. |
| `RightIsTracking` | **[ValueStream\`1](https://wiki.resonite.com/index.php?title=Type:ValueStream%601&action=edit&redlink=1 "Type:ValueStream`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >** | The stream data for the right hand. |
| `Stream` | **[MultiValueStream\`1](https://wiki.resonite.com/index.php?title=Type:MultiValueStream%601&action=edit&redlink=1 "Type:MultiValueStream`1 (page does not exist)") < [FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ") >** | The stream data from all the tracking. |
| `TracksMetacarpals` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Should the metacarpals be tracked. |
| `PoseController` | **[UserPoseController](https://wiki.resonite.com/Component:UserPoseController "Component:UserPoseController")** | The pose controller from the user. |

Fields
Collapse

## Usage

Used for [Finger Posing System](https://wiki.resonite.com/Finger_Posing_System "Finger Posing System").

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:FingerPoseStreamManager&oldid=97343](https://wiki.resonite.com/index.php?title=Component:FingerPoseStreamManager&oldid=97343)"

Contents