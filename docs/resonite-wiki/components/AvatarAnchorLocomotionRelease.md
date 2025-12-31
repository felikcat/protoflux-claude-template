# Component:AvatarAnchorLocomotionRelease

> Source: https://wiki.resonite.com/Component:AvatarAnchorLocomotionRelease

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:AvatarAnchorLocomotionRelease&diff=93284) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/2/2b/AvatarAnchorLocomotionReleaseComponent.png/510px-AvatarAnchorLocomotionReleaseComponent.png)](https://wiki.resonite.com/File:AvatarAnchorLocomotionReleaseComponent.png) **Avatar Anchor Locomotion Release** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **AvatarAnchorLocomotionRelease** Component is used so a user can get out of an anchor with their controller when they get into an anchor.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `ReleaseOnBinaryAction` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to allow the user to jump out of the anchor |
| `ReleaseStrengthThreshold` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | The amount of pressing strength on the jump button needed to get out if not null. |

Fields
Collapse

## Usage

Has to be used on the same slot as an [Component:AvatarAnchor](https://wiki.resonite.com/Component:AvatarAnchor "Component:AvatarAnchor") or it doesn't do anything.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Component:AvatarAnchor](https://wiki.resonite.com/Component:AvatarAnchor "Component:AvatarAnchor")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AvatarAnchorLocomotionRelease&oldid=93284](https://wiki.resonite.com/index.php?title=Component:AvatarAnchorLocomotionRelease&oldid=93284)"

Contents