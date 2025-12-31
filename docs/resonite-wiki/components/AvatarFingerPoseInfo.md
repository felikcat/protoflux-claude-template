# Component:AvatarFingerPoseInfo

> Source: https://wiki.resonite.com/Component:AvatarFingerPoseInfo

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:AvatarFingerPoseInfo&diff=93715) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/e/e1/AvatarFingerPoseInfoComponent.png/510px-AvatarFingerPoseInfoComponent.png)](https://wiki.resonite.com/File:AvatarFingerPoseInfoComponent.png) **AvatarFingerPoseInfo** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **AvatarFingerPoseInfo** is used to override the assigning behavior from a [Component:AvatarHandDataAssigner](https://wiki.resonite.com/Component:AvatarHandDataAssigner "Component:AvatarHandDataAssigner") on the avatar when it assigns a target.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `FingerPoseSource` | **[IFingerPoseSourceComponent](https://wiki.resonite.com/Type:IFingerPoseSourceComponent "Type:IFingerPoseSourceComponent")** | The data source to override the assigning behavior of a [Component:AvatarHandDataAssigner](https://wiki.resonite.com/Component:AvatarHandDataAssigner "Component:AvatarHandDataAssigner") on the avatar with. |

Fields
Collapse

## Usage

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AvatarFingerPoseInfo&oldid=93715](https://wiki.resonite.com/index.php?title=Component:AvatarFingerPoseInfo&oldid=93715)"

Contents