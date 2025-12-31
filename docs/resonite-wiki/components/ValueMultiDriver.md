# Component:ValueMultiDriver

> Source: https://wiki.resonite.com/Component:ValueMultiDriver

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:ValueMultiDriver&diff=94982) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/a/a6/ValueMultiDriver%601Component.png/510px-ValueMultiDriver%601Component.png)](https://wiki.resonite.com/File:ValueMultiDriver%601Component.png) **ValueMultiDriver\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ValueMultiDriver\`1** component allows you to drive multiple fields from a single value.

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Value` | **T** | Value of the specified type, which will be driven to all fields listed in `Drives` |
| `Drives` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[FieldDrive\`1](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1") <T>** | A list of fields to be driven by this component |

Fields
Collapse

## Behavior

## Examples

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ValueMultiDriver&oldid=94982](https://wiki.resonite.com/index.php?title=Component:ValueMultiDriver&oldid=94982)"

Contents