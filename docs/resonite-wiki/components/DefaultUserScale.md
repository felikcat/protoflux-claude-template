# Component:DefaultUserScale

> Source: https://wiki.resonite.com/Component:DefaultUserScale

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:DefaultUserScale&diff=91228) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/d/d6/DefaultUserScaleComponent.png/510px-DefaultUserScaleComponent.png)](https://wiki.resonite.com/File:DefaultUserScaleComponent.png) **DefaultUserScale** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

This component sets the default scale of the avatar it is attached to, which also affects the scale of the user wearing said avatar.

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `SetOnEquip` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | TBD |
| `DefaultScale` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The default scale (normal value is 1) |
| `_activeUser` | **[User](https://wiki.resonite.com/Type:User "Type:User")** | Internal |

Fields
Collapse

## Behavior

The default scale determines what scale the avatar spawns at, as well as what scale it returns to when using the _Reset Scale_ option in the context menu.

## Examples

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:DefaultUserScale&oldid=91228](https://wiki.resonite.com/index.php?title=Component:DefaultUserScale&oldid=91228)"

Contents