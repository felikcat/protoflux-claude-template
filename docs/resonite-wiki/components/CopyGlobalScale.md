# Component:CopyGlobalScale

> Source: https://wiki.resonite.com/Component:CopyGlobalScale

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:CopyGlobalScale&diff=91213) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/b/b1/CopyGlobalScaleComponent.png/510px-CopyGlobalScaleComponent.png)](https://wiki.resonite.com/File:CopyGlobalScaleComponent.png) **Copy Global Scale** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The CopyGlobalScale component is used to ensure that one object has the exact same global scale as another object.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Source` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The object that serves as scale reference. |
| `NonUniform` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | If true, non-uniform scale is preserved, otherwise the X scale of the source serves as X, Y and Z of the target. |
| `_scaleDrive` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field that is driven to match the global scale of the source. This automatically gets populated with the scale field of the slot that this component is added to. |

Fields
Collapse

## Usage

## Examples

## Related Issues

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:CopyGlobalScale&oldid=91213](https://wiki.resonite.com/index.php?title=Component:CopyGlobalScale&oldid=91213)"

Contents