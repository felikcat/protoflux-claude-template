# Component:Grabber

> Source: https://wiki.resonite.com/Component:Grabber

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:Grabber&diff=96756) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/c/c2/GrabberComponent.png/510px-GrabberComponent.png)](https://wiki.resonite.com/File:GrabberComponent.png) **Grabber** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

Grabber is a Component that is used in a [User](https://wiki.resonite.com/User "User")'s hiearchy to allow the user to grab objects. This component is generated internally usually. Interacting with this component dynamically is done through [Grabbable ProtoFlux Nodes](https://wiki.resonite.com/Category:ProtoFlux:Interaction:Grabbable "Category:ProtoFlux:Interaction:Grabbable").

[Frooxius](https://wiki.resonite.com/User:Frooxius "User:Frooxius") mentioned if a foot grabbing tracking device was made for wide consumer use, they would add it as a possible Grabber node. [\[1\]](https://wiki.resonite.com/Component:Grabber#cite_note-1)

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `AutoUpdateUser` | **[User](https://wiki.resonite.com/Type:User "Type:User")** | The user handling updates for this Grabber. |
| `ReleaseCheckRadius` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How far to check before releasing a grabbable from the `_baseDistance`. Usually used for dynamic bones. |
| `CorrespondingBodyNode` | **[BodyNode](https://wiki.resonite.com/Type:BodyNode "Type:BodyNode")** | The node this hand is associated with. |
| `_scaleReference` | **Grabber** | The grabber used as a scale reference, like the opposite hand. |
| `_baseScale` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The default scale for the grabber. |
| `_baseDistance` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The default distance for the grabber. |
| `_holderSlot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot used to store objects being grabbed by the user. |

Fields
Collapse

## Usage

This component can be triggered to grab things by the user. However, this requires a [Component:TrackedHand](https://wiki.resonite.com/Component:TrackedHand "Component:TrackedHand") to be attached under the user, or be part of an avatar spawned onto them. The tracked hand then auto generates this component. However, the component only will grab things when that tracked hand component detects that the user associated with it is trying to grab using the hand side it is assigned to. This does allow for multiple grabbers on the same hand however.

## Examples

Used on the user's grab anchor slots on their hands to allow the user to grab things.

## See Also

- [Component:Grabbable](https://wiki.resonite.com/Component:Grabbable "Component:Grabbable")

1. [↑](https://wiki.resonite.com/Component:Grabber#cite_ref-1 "Jump up")This was mentioned in a YouTube video. Citation needed!

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:Grabber&oldid=96756](https://wiki.resonite.com/index.php?title=Component:Grabber&oldid=96756)"

Contents