# Component:TimeIntDriver

> Source: https://wiki.resonite.com/Component:TimeIntDriver

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:TimeIntDriver&diff=92346) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/d/dc/TimeIntDriverComponent.png/510px-TimeIntDriverComponent.png)](https://wiki.resonite.com/File:TimeIntDriverComponent.png) **TimeIntDriver** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **TimeIntDriver** Component drives the [Int](https://wiki.resonite.com/Type:Int "Type:Int") value specified in `Target` based on the current time, modified by the specified parameters.

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Scale` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Time scale in relation to time in seconds, where 1.0 means `Target` will increment once per second. |
| `Repeat` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Once `Target` reaches this value, it will reset to 0 and restart. |
| `PingPong` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Causes `Target` to reverse direction when it reaches 0 or the value in `Repeat`, instead of restarting. |
| `Target` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The value to be driven. |

Fields
Collapse

## Usage

Can be used with [Component:UVAtlasAnimator](https://wiki.resonite.com/Component:UVAtlasAnimator "Component:UVAtlasAnimator") to constantly drive the animation of a material.

## Examples

- [TimeIntDriver for Integer Animations](https://www.youtube.com/watch?v=Nbnx23oGtXo) by [ProbablePrime](https://wiki.resonite.com/User:ProbablePrime "User:ProbablePrime")

## Related Components

- [Component:AtlasInfo](https://wiki.resonite.com/Component:AtlasInfo "Component:AtlasInfo")
- Component:TimeIntDriver
- [Component:UVAtlasAnimator](https://wiki.resonite.com/Component:UVAtlasAnimator "Component:UVAtlasAnimator")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:TimeIntDriver&oldid=92346](https://wiki.resonite.com/index.php?title=Component:TimeIntDriver&oldid=92346)"

Contents