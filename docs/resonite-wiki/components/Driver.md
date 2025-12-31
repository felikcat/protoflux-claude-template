# Component:Driver

> Source: https://wiki.resonite.com/Component:Driver

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/6/68/Driver%601Component.png/510px-Driver%601Component.png)](https://wiki.resonite.com/File:Driver%601Component.png) **Driver\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Driver** component drives a value field via a protoflux output. This is used in [ProtoFlux](https://wiki.resonite.com/ProtoFlux "ProtoFlux") to utilize output calculations.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Source` | **[INodeOutput\`1](https://wiki.resonite.com/index.php?title=Type:INodeOutput%601&action=edit&redlink=1 "Type:INodeOutput`1 (page does not exist)") <T>** | The node output to get a value from. |
| `Target` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **T** | The value to drive with the output acquired from `Source`. |

Fields
Collapse

## Usage

Not used by the user directly, but is made by Flux drivers.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:Driver&oldid=96456](https://wiki.resonite.com/index.php?title=Component:Driver&oldid=96456)"

Contents