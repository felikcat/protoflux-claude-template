# Component:AvatarLiveIndicator

> Source: https://wiki.resonite.com/Component:AvatarLiveIndicator

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:AvatarLiveIndicator&diff=91179) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/2/27/AvatarLiveIndicatorComponent.png/510px-AvatarLiveIndicatorComponent.png)](https://wiki.resonite.com/File:AvatarLiveIndicatorComponent.png) **AvatarLiveIndicator** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **AvatarLiveIndicator** component is used to show or enable a [slot](https://wiki.resonite.com/Slot "Slot") (usually a visual) to let other [users](https://wiki.resonite.com/User "User") know that you are live. This activates from the [streaming camera control panel](https://wiki.resonite.com/Camera#Photo_Controls "Camera"), specifically the "Mirror to display" button.

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `IsLive` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether `_activeUser` is streaming or not. |
| `_activeUser` | **[User](https://wiki.resonite.com/Type:User "Type:User")** | The user that this component is monitoring |

Fields
Collapse

## Usage

Usually this is used with the [Camera](https://wiki.resonite.com/Camera "Camera"), especially when streaming. This is also already setup along with the [Nameplate](https://wiki.resonite.com/Nameplate "Nameplate") and positioned on it (however, this can be customizable).

## Examples

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AvatarLiveIndicator&oldid=91179](https://wiki.resonite.com/index.php?title=Component:AvatarLiveIndicator&oldid=91179)"

Contents