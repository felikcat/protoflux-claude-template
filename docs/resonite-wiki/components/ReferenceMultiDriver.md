# Component:ReferenceMultiDriver

> Source: https://wiki.resonite.com/Component:ReferenceMultiDriver

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:ReferenceMultiDriver&diff=82480) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/2/2f/ReferenceMultiDriver%601Component.png/510px-ReferenceMultiDriver%601Component.png)](https://wiki.resonite.com/File:ReferenceMultiDriver%601Component.png) **ReferenceMultiDriver\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ReferenceMultiDriver\`1** component allows you to drive multiple fields from a single reference.

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Reference` | **T** | Reference of the specified type, which will be driven to all fields listed in `Drives` |
| `Drives` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[RefDrive\`1](https://wiki.resonite.com/index.php?title=Type:RefDrive%601&action=edit&redlink=1 "Type:RefDrive`1 (page does not exist)") <T>** | A list of fields to be driven by this component |

Fields
Collapse

## Behavior

## Examples

## Related Issues

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ReferenceMultiDriver&oldid=82480](https://wiki.resonite.com/index.php?title=Component:ReferenceMultiDriver&oldid=82480)"

Contents