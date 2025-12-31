# Component:GrabbableParenter

> Source: https://wiki.resonite.com/Component:GrabbableParenter

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:GrabbableParenter&diff=96699) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/8/8a/GrabbableParenterComponent.png/510px-GrabbableParenterComponent.png)](https://wiki.resonite.com/File:GrabbableParenterComponent.png) **Grabbable Parenter** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

Grabbable Parenter is a component that when paired with a [collider](https://wiki.resonite.com/Collider "Collider") that is not set to a Trigger or StaticTrigger type, it will receive objects that are released within it's collider. This is a volume based alternative to [Grabbable Receiver Surface](https://wiki.resonite.com/Component:GrabbableReceiverSurface "Component:GrabbableReceiverSurface").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `ParentUnder` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot to parent objects under instead of the slot this component is on. |
| `Filter` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[Func\`2](https://wiki.resonite.com/Type:Func%602 "Type:Func`2") < [IGrabbable](https://wiki.resonite.com/Type:IGrabbable "Type:IGrabbable"), [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >** | A [Sync Delegate](https://wiki.resonite.com/Sync_Delegate "Sync Delegate") that takes an [IGrabbable](https://wiki.resonite.com/Type:IGrabbable "Type:IGrabbable") and returns a [boolean](https://wiki.resonite.com/Type:Bool "Type:Bool"). If a grabbable returns false when fed into this function, that IGrabbable will not be parented by this component. |

Fields
Collapse

## Behavior

Unlike [Grabbable Receiver Surface](https://wiki.resonite.com/Component:GrabbableReceiverSurface "Component:GrabbableReceiverSurface"), [Grabbable](https://wiki.resonite.com/Component:Grabbable "Component:Grabbable") objects parented to this Slot will be reparented to it when dropped outside of its collider. This can be prevented with the [GrabbableReparentBlock](https://wiki.resonite.com/Component:GrabbableReparentBlock "Component:GrabbableReparentBlock") component.

## Examples

[ProbablePrime](https://wiki.resonite.com/User:ProbablePrime "User:ProbablePrime")'s tutorial on GrabbableParenter:

![](https://i.ytimg.com/vi/sEAePnKuXGk/hqdefault.jpg)

[OLD: Neos VR Tutorial: GrabbableParenter](https://www.youtube-nocookie.com/embed/sEAePnKuXGk?autoplay=1)

Load video

YouTube

YouTube might collect personal data. [Privacy Policy](https://www.youtube.com/howyoutubeworks/user-settings/privacy/)

ContinueDismiss

## See Also

- [Grabbable](https://wiki.resonite.com/Component:Grabbable "Component:Grabbable")
- [Component:GrabbableReceiverSurface](https://wiki.resonite.com/Component:GrabbableReceiverSurface "Component:GrabbableReceiverSurface")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:GrabbableParenter&oldid=96699](https://wiki.resonite.com/index.php?title=Component:GrabbableParenter&oldid=96699)"

Contents