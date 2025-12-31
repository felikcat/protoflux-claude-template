# Component:ColliderUserTracker

> Source: https://wiki.resonite.com/Component:ColliderUserTracker

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/b/b3/ColliderUserTrackerComponent.png/510px-ColliderUserTrackerComponent.png)](https://wiki.resonite.com/File:ColliderUserTrackerComponent.png) **Collider User Tracker** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ColliderUserTracker** keeps track of users who enter and leave a collider. It must be used on a Slot that also has an attached Collider whose type is set to "Trigger", unless `TriggersOnly` is set to false.

As this component works using colliders, it cannot detect users in No-Clip.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `TriggersOnly` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to only allow use of Triggers or not. |
| `IsLocalUserInside` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Becomes set for the local user if the local user is within the collider of the object that this component is attached to. |
| `IsAnyUserInside` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Becomes set for all users if any user is within the collider of the object that this component is attached to. |
| `NumberOfUsersInside` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Tracks the number of users inside the collider of the object that this component is attached to. |
| `_usersInside` | _[unordered list](https://wiki.resonite.com/Type:SyncBag%601 "Type:SyncBag`1")_ of **[UserRef](https://wiki.resonite.com/Type:UserRef "Type:UserRef")** | Data on the users that are inside the collider of the object that this component is attached to. |

Fields
Collapse

## Usage

Attach this component to a slot, and add a [Collider](https://wiki.resonite.com/index.php?title=Colliders&action=edit&redlink=1 "Colliders (page does not exist)") to the slot. The component will then start functioning as long as the Collider is a trigger or as long as `TriggersOnly` is set to false.

## Examples

This component can be very useful in defining zones in a world for various features, the most common of which is using the `IsLocalUserInside` to drive the Enabled state on various slots to work as a culling system.

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ColliderUserTracker&oldid=91252](https://wiki.resonite.com/index.php?title=Component:ColliderUserTracker&oldid=91252)"

Contents