# Component:AvatarNeckOffset

> Source: https://wiki.resonite.com/Component:AvatarNeckOffset

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/f/f4/AvatarNeckOffsetComponent.png/510px-AvatarNeckOffsetComponent.png)](https://wiki.resonite.com/File:AvatarNeckOffsetComponent.png) **AvatarNeckOffset** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

Avatar Neck Offset is a component that allows for dynamically lengthening and shortening the neck of an avatar.

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Priority` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | How much priority this component takes over other components that constrain or change [Avatar Pose Nodes](https://wiki.resonite.com/Component:AvatarPoseNode "Component:AvatarPoseNode") |
| `Offset` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | How much to offset the user's neck from it's original position in local space. |
| `_activeUser` | **[User](https://wiki.resonite.com/Type:User "Type:User")** | Internal. Automatically updates to active user of this component that's being affected by it. |

Fields
Collapse

## Behavior

The effect of this component when used updates instantly.

## Examples

This is used in a silly user created item dubbed "the giraffe hat" that lengthens the user's neck when worn on their head.

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AvatarNeckOffset&oldid=91175](https://wiki.resonite.com/index.php?title=Component:AvatarNeckOffset&oldid=91175)"

Contents