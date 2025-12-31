# Component:TestFakeViveTracker

> Source: https://wiki.resonite.com/Component:TestFakeViveTracker

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/5/54/TestFakeViveTrackerComponent.png/510px-TestFakeViveTrackerComponent.png)](https://wiki.resonite.com/File:TestFakeViveTrackerComponent.png) **Test Fake Vive Tracker** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **TestFakeViveTracker** component simulates a vive Tracker for `User` that has the position and rotation of the slot this component is on. This allows for making fake trackers that can be used to control the `User`'s IK as a real Tracker would. It even """tricks""" the input system into fully seeing this as a Tracker, even generating a visual for the user. The tracker device's position/rotation is based on its position/rotation in global space compared to `User`'s root slot global position/rotation.

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This game element is a debug item. Elements like this may be removed at any time without warning, and creations should not rely on it.


## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Id` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | Upon attaching is a random GUID. Can be changed which makes a new Tracker object. If identical to another older tracker the user has used before, will take on the old tracker's identity and settings. |
| `IsTracking` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether the tracker has lost tracking. |
| `User` | _direct_ **[UserRef](https://wiki.resonite.com/Type:UserRef "Type:UserRef")** | The user this tracker shoul |

Fields
Collapse

## Usage

Attach to a slot and preferably parent it under the `User` to create a new tracker for the targeted `User`. a user is needed for this component to work.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:TestFakeViveTracker&oldid=96377](https://wiki.resonite.com/index.php?title=Component:TestFakeViveTracker&oldid=96377)"

Contents