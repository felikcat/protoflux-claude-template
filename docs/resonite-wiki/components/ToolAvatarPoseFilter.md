# Component:ToolAvatarPoseFilter

> Source: https://wiki.resonite.com/Component:ToolAvatarPoseFilter

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:ToolAvatarPoseFilter&diff=93824) which are not marked for translation.

Collapse **Component image**

[File:ToolAvatarPoseFilterComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=ToolAvatarPoseFilterComponent.png "File:ToolAvatarPoseFilterComponent.png") **Tool Avatar Pose Filter** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ToolAvatarPoseFilter** component is used to assign a Pose Filter to the hand you have a Tool equipped on.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Filter` | **[IAvatarPoseFilter](https://wiki.resonite.com/Type:IAvatarPoseFilter "Type:IAvatarPoseFilter")** | The pose filter to apply |
| `Priority` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Whether this pose filter should be applied before other filters. |

Fields
Collapse

## Usage

This can be used on any type of tool.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Component:GrabbableAvatarPoseFilter](https://wiki.resonite.com/Component:GrabbableAvatarPoseFilter "Component:GrabbableAvatarPoseFilter")
- [Component:AvatarAnchor](https://wiki.resonite.com/Component:AvatarAnchor "Component:AvatarAnchor")
- Component:ToolAvatarPoseFilter
- [Component:AvatarPoseOffset](https://wiki.resonite.com/Component:AvatarPoseOffset "Component:AvatarPoseOffset")
- [Component:AvatarPoseSmoothLerp](https://wiki.resonite.com/Component:AvatarPoseSmoothLerp "Component:AvatarPoseSmoothLerp")
- [Component:AvatarPoseRotationConstraint](https://wiki.resonite.com/Component:AvatarPoseRotationConstraint "Component:AvatarPoseRotationConstraint")
- [Component:AvatarPoseBoxConstraint](https://wiki.resonite.com/Component:AvatarPoseBoxConstraint "Component:AvatarPoseBoxConstraint")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ToolAvatarPoseFilter&oldid=93824](https://wiki.resonite.com/index.php?title=Component:ToolAvatarPoseFilter&oldid=93824)"

Contents