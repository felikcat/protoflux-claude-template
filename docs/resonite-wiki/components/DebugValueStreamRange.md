# Component:DebugValueStreamRange

> Source: https://wiki.resonite.com/Component:DebugValueStreamRange

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/c/c5/DebugValueStreamRangeComponent.png/510px-DebugValueStreamRangeComponent.png)](https://wiki.resonite.com/File:DebugValueStreamRangeComponent.png) **Debug Value Stream Range** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **DebugValueStreamRange** component is used to debug the range of a Float3 stream for debugging. Like a graph of sorts.

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This game element is a debug item. Elements like this may be removed at any time without warning, and creations should not rely on it.


## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Stream` | **[ValueStream\`1](https://wiki.resonite.com/index.php?title=Type:ValueStream%601&action=edit&redlink=1 "Type:ValueStream`1 (page does not exist)") < [Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3") >** | The stream to debug. |
| `positionDrive` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The position field to drive with the stream position. |
| `sizeDrive` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to drive with the overall stream range. |

Fields
Collapse

## Usage

Not generally useful to the user.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:DebugValueStreamRange&oldid=96435](https://wiki.resonite.com/index.php?title=Component:DebugValueStreamRange&oldid=96435)"

Contents