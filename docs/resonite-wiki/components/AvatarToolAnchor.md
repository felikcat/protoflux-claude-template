# Component:AvatarToolAnchor

> Source: https://wiki.resonite.com/Component:AvatarToolAnchor

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:AvatarToolAnchor&diff=97399) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/3/33/AvatarToolAnchorComponent.png/510px-AvatarToolAnchorComponent.png)](https://wiki.resonite.com/File:AvatarToolAnchorComponent.png) **AvatarToolAnchor** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

Avatar Tool anchor is a component that defines where to place either the tool, toolshelf, or grab area anchors when the avatar is equipped. Or where to position the context menu when it is opened.

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `AnchorPoint` | **[AvatarToolAnchor.Point](https://wiki.resonite.com/Component:AvatarToolAnchor#Point)** | The type of tool anchor to place under the slot this component is on for this hand. |

Fields
Collapse

## Point

| Name | Value | Description |
| --- | --- | --- |
| `Tool` | 1 | Place the tooltip anchor for this hand here. |
| `GrabArea` | 2 | Place the grabber sphere anchor for this hand here. |
| `Toolshelf` | 3 | Place the toolshelf anchor for this hand here. |
| `Menu` | 4 | Position the context menu here when it is opened on this hand here. |
| `Tooltip` | 0 | Used to be used, OBSOLETE. |

Values

## Behavior

## Examples

Is automatically placed on avatars upon avatar creation on the hands. Can be moved to say the mouth, to allow grabbing objects with the mouth using the hand for which the anchor came from. Driving the parent value of the slot this component is on is an efficient way of doing this.

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AvatarToolAnchor&oldid=97399](https://wiki.resonite.com/index.php?title=Component:AvatarToolAnchor&oldid=97399)"

Contents