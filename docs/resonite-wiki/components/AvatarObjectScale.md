# Component:AvatarObjectScale

> Source: https://wiki.resonite.com/Component:AvatarObjectScale

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:AvatarObjectScale&diff=91578) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/9/98/AvatarObjectScaleComponent.png/510px-AvatarObjectScaleComponent.png)](https://wiki.resonite.com/File:AvatarObjectScaleComponent.png) **AvatarObjectScale** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **AvatarObjectScale** component allows setting it's slot scale relative to the UserRoot slot when equipped under an avatar.

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `UserSpaceScale` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The desired scale relative to the UserRoot slot. |

Fields
Collapse

## Behavior

On equip the component will set the attached slot scale to be `UserSpaceScale` in the UserRoot slot space.

## Examples

## Related Issues

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AvatarObjectScale&oldid=91578](https://wiki.resonite.com/index.php?title=Component:AvatarObjectScale&oldid=91578)"

Contents