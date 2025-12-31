# Component:DestroyOnUserLeave

> Source: https://wiki.resonite.com/Component:DestroyOnUserLeave

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:DestroyOnUserLeave&diff=81820) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/a/a4/DestroyOnUserLeaveComponent.png/510px-DestroyOnUserLeaveComponent.png)](https://wiki.resonite.com/File:DestroyOnUserLeaveComponent.png) **DestroyOnUserLeave** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **DestroyOnUserLeave** component causes the parent slot to be deleted when the user specified in `User` leaves the world.

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `TargetUser` | _direct_ **[UserRef](https://wiki.resonite.com/Type:UserRef "Type:UserRef")** | The user that will cause the parent slot to be deleted upon leaving |

Fields
Collapse

## Behavior

## Examples

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:DestroyOnUserLeave&oldid=81820](https://wiki.resonite.com/index.php?title=Component:DestroyOnUserLeave&oldid=81820)"

Contents