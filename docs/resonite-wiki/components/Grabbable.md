# Component:Grabbable

> Source: https://wiki.resonite.com/Component:Grabbable

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/0/0c/GrabbableComponent.png/510px-GrabbableComponent.png)](https://wiki.resonite.com/File:GrabbableComponent.png) **Grabbable** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

> Grabbable is a complicated thing
>
> — AlexFromAlaska

The **Grabbable** component allows you to grab any slot it is attached to, provided it has some type of [Collider](https://wiki.resonite.com/Collider "Collider").

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `ReparentOnRelease` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | The slot is reparented to the value of `_lastParent`, instead of root when dropped **\*** |
| `PreserveUserSpace` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | The slot is reparented to [Local User Space](https://wiki.resonite.com/index.php?title=Local_User_Space&action=edit&redlink=1 "Local User Space (page does not exist)") **\*** |
| `DestroyOnRelease` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | The slot this component is attached to is destroyed upon release |
| `GrabPriority` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Determines what gets grabbed if several grabbable objects are touching someone's grab sphere. The [IGrabbable](https://wiki.resonite.com/Type:IGrabbable "Type:IGrabbable") with the highest priority will be grabbed first. If the highest priority ties with another [IGrabbable](https://wiki.resonite.com/Type:IGrabbable "Type:IGrabbable"), it will grab both of those and ignore any lower priority [IGrabbables](https://wiki.resonite.com/Type:IGrabbable "Type:IGrabbable"). |
| `GrabPriorityWhenGrabbed` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Int](https://wiki.resonite.com/Type:Int "Type:Int") >** | Optionally changes the grab priority of the object when it is already being grabbed. Useful for different behavior when it can be grab stolen by another player. |
| `CustomCanGrabCheck` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[GrabCheck](https://wiki.resonite.com/Type:GrabCheck "Type:GrabCheck")** | _Not Usable inside Resonite_ Requires a mod for interacting with [Sync Delegates](https://wiki.resonite.com/Sync_Delegates "Sync Delegates") |
| `EditModeOnly` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines if this grabbable is effective only in [Edit Mode](https://wiki.resonite.com/Edit_Mode "Edit Mode") |
| `AllowSteal` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Other users can grab the slot this component is attached to. Like a flag in capture the flag. |
| `DropOnDisable` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | The parent slot will be dropped when this component is disabled. |
| `ActiveUserFilter` | **[ActiveUserHandling](https://wiki.resonite.com/Type:ActiveUserHandling "Type:ActiveUserHandling")** | Changes if this component can be grabbed based on who is the active user if any. |
| `OnlyUsers` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[UserRef](https://wiki.resonite.com/Type:UserRef "Type:UserRef")** | A list of users that are allowed to grab this slot. |
| `Scalable` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Scalable determines if the grabbable's slot can be scaled. |
| `Receivable` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Receivable determines if a grabbable can be dropped onto a [GrabbableReceiverSurface](https://wiki.resonite.com/GrabbableReceiverSurface_(Component) "GrabbableReceiverSurface (Component)") when let go of. The receivable has to be close enough for the receiver to receive it. |
| `AllowOnlyPhysicalGrab` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Only allow grab an object with a physical interaction - remote grabs are not allowed |
| `_grabber` | **[Grabber](https://wiki.resonite.com/Component:Grabber "Component:Grabber")** | _Automatically Assigned_, the grabber that is grabbing this component. |
| `_lastParent` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | _Automatically Assigned_, the last parent this slot had. Is used to parent the slot back (if allowed) when let go of. |
| `_lastParentIsUserSpace` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | _Automatically Assigned_ Whether the last parent slot is the user space slot of the user grabbing this. |
| `__legacyActiveUserRootOnly` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | _Automatically Assigned_ Legacy do not use. Used to handle whether only the active user can grab. Use `ActiveUserFilter` instead! |

Fields
Collapse

## Behavior

The interaction between `ReparentOnRelease`, `PreserveUserSpace` and any [Grabbable extensions](https://wiki.resonite.com/index.php?title=Category:Grabbable_extensions&action=edit&redlink=1 "Category:Grabbable extensions (page does not exist)"), such as [GrabbableReparentBlock](https://wiki.resonite.com/Component:GrabbableReparentBlock "Component:GrabbableReparentBlock"), is somewhat complex.

When released, the following will be evaluated, in order:

1. If `ReparentOnRelease` is true, the slot will be parented to the value in `_lastParent`
2. If `PreserveUserSpace` and `_lastParentIsUserSpace` is true, the slot will be parented to [Local User Space](https://wiki.resonite.com/ProtoFlux:LocalUserSpace "ProtoFlux:LocalUserSpace")
3. If an [IGrabbable](https://wiki.resonite.com/Type:IGrabbable "Type:IGrabbable") exists above this component in the hierarchy, and it is within the `MaxDepth` specified in the block, the slot will be parented to Local User Space
4. Otherwise, the slot is parented to root.

* * *

You can drive the scale of a Grabbable object if the `Scalable` boolean is false.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [IGrabbable](https://wiki.resonite.com/Type:IGrabbable "Type:IGrabbable") for a list of grabbable types that act similar but not the same as this component.

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:Grabbable&oldid=113345](https://wiki.resonite.com/index.php?title=Component:Grabbable&oldid=113345)"

Contents