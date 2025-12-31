# Component:GrabInstancer

> Source: https://wiki.resonite.com/Component:GrabInstancer

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:GrabInstancer&diff=94778) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/1/17/GrabInstancerComponent.png/510px-GrabInstancerComponent.png)](https://wiki.resonite.com/File:GrabInstancerComponent.png) **GrabInstancer** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **GrabInstancer** component spawns a new copy of `Template` and attaches it to the user's hand whenever the slot it is attached to is grabbed.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Template` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot that gets duplicated and grabbed when the GrabInstancer is grabbed. (Like a figurine) |
| `ContainerTemplate` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot to duplicate and act as a container for the grabbed object (Like a box for a figurine) |
| `ContainerTemplateInstanceRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The override on where to place the duplicated grabbed object (Where to put the figurine in the box hiearchy). |
| `ActivateRoot` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether or not the GrabInstancer should activate the newly duplicated slot. |
| `EnableGrabbable` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether or not the GrabInstancer should activate any Grabbable component on the newly duplicated slot. |
| `SetInstancePersistent` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >** | Whether to set the duplicated object's persistence field, and what to set it to. |
| `ExcludedParts` | _[list](https://wiki.resonite.com/Type:SyncRefList%601 "Type:SyncRefList`1")_ of **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | slots will be skipped while duplicating |
| `Physical` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | If true, the GrabInstancer only reacts to physical grab. |
| `GrabPriority` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Determines what gets grabbed if several grabbable objects are touching someone's grab sphere. The [IGrabbable](https://wiki.resonite.com/Type:IGrabbable "Type:IGrabbable") with the highest priority will be grabbed first. If the highest priority ties with another [IGrabbable](https://wiki.resonite.com/Type:IGrabbable "Type:IGrabbable"), it will grab both of those and ignore any lower priority [IGrabbables](https://wiki.resonite.com/Type:IGrabbable "Type:IGrabbable"). |

Fields
Collapse

## Usage

Attach to a slot and provide a value for `Template` at minimum.

## Examples

A video tutorial about the GrabInstancer by [ProbablePrime](https://wiki.resonite.com/User:ProbablePrime "User:ProbablePrime"):

![](https://i.ytimg.com/vi/QFWU2dZTDvw/hqdefault.jpg)

[OLD: Neos VR Tutorial: GrabInstancer](https://www.youtube-nocookie.com/embed/QFWU2dZTDvw?autoplay=1)

Load video

YouTube

YouTube might collect personal data. [Privacy Policy](https://www.youtube.com/howyoutubeworks/user-settings/privacy/)

ContinueDismiss

## See Also

- [UIGrabInstancer](https://wiki.resonite.com/Component:UIGrabInstancer "Component:UIGrabInstancer") is similar to this component but uses [UIX](https://wiki.resonite.com/UIX "UIX") elements to do this.

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:GrabInstancer&oldid=94778](https://wiki.resonite.com/index.php?title=Component:GrabInstancer&oldid=94778)"

Contents