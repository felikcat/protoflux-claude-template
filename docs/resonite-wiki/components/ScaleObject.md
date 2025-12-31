# Component:ScaleObject

> Source: https://wiki.resonite.com/Component:ScaleObject

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:ScaleObject&diff=96148) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/3/34/ScaleObjectComponent.png/510px-ScaleObjectComponent.png)](https://wiki.resonite.com/File:ScaleObjectComponent.png) **Scale Object** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ScaleObject** component can be used to position and scale a slot relative to a [ScaleObjectManager](https://wiki.resonite.com/Component:ScaleObjectManager "Component:ScaleObjectManager").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Manager` | **[ScaleObjectManager](https://wiki.resonite.com/Component:ScaleObjectManager "Component:ScaleObjectManager")** |  |
| `ScalePower` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** |  |
| `ScalePosition` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** |  |
| `OverrideFarTransitionOffset` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3") >** |  |
| `CustomTransition` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** |  |
| `TransitionLerp` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** |  |
| `_active` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** |  |
| `_position` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** |  |
| `_scale` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** |  |

Fields
Collapse

## Usage

## Examples

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ScaleObject&oldid=96148](https://wiki.resonite.com/index.php?title=Component:ScaleObject&oldid=96148)"

Contents