# Component:GrabbableReparentBlock

> Source: https://wiki.resonite.com/Component:GrabbableReparentBlock

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:GrabbableReparentBlock&diff=98517) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/6/62/GrabbableReparentBlockComponent.png/510px-GrabbableReparentBlockComponent.png)](https://wiki.resonite.com/File:GrabbableReparentBlockComponent.png) **Grabbable Reparent Block** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **GrabbableReparentBlock** component prevents any [slot](https://wiki.resonite.com/Slot "Slot") [tagged](https://wiki.resonite.com/Tag "Tag") by this component below it in the hierarchy, up to `MaxDepth` levels deep, from being reparented to any slot above it.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `DontReparent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Don't allow this slot to be reparented. Subject to the rules explained in [Grabbable - Behavior](https://wiki.resonite.com/Component:Grabbable#Behavior "Component:Grabbable") |
| `MaxDepth` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Objects beyond this level in the hierarchy will not be effected. Set to [Int MaxValue](https://wiki.resonite.com/Type:Int "Type:Int") by default |

Fields
Collapse

## Usage

## Examples

- **GrabbableReparentBlock** by [ProbablePrime](https://wiki.resonite.com/User:ProbablePrime "User:ProbablePrime")

![](https://i.ytimg.com/vi/Da0VJ0hFn_0/hqdefault.jpg)

[OLD: Neos VR Tutorial: GrabbableReparentBlock](https://www.youtube-nocookie.com/embed/Da0VJ0hFn_0?autoplay=1)

Load video

YouTube

YouTube might collect personal data. [Privacy Policy](https://www.youtube.com/howyoutubeworks/user-settings/privacy/)

ContinueDismiss

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:GrabbableReparentBlock&oldid=98517](https://wiki.resonite.com/index.php?title=Component:GrabbableReparentBlock&oldid=98517)"

Contents