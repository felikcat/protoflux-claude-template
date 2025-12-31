# Component:ButtonReferenceCycle

> Source: https://wiki.resonite.com/Component:ButtonReferenceCycle

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:ButtonReferenceCycle&diff=90358) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/d/dc/ButtonReferenceCycle%601Component.png/510px-ButtonReferenceCycle%601Component.png)](https://wiki.resonite.com/File:ButtonReferenceCycle%601Component.png) **Button Reference Cycle\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ButtonReferenceCycle** component holds a list of [references](https://wiki.resonite.com/Reference_Types "Reference Types") and takes in a `TargetReference` of a provided type. When an [IButton](https://wiki.resonite.com/Type:IButton "Type:IButton") is pressed while this component is on it, this will cycle through the listed references and send the data through the `TargetReference`.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `TargetReference` | **[SyncRef\`1](https://wiki.resonite.com/Type:SyncRef%601 "Type:SyncRef`1") <T>** | The reference data to send outwards. |
| `Targets` | _[list](https://wiki.resonite.com/Type:SyncRefList%601 "Type:SyncRefList`1")_ of **T** | The list of references to cycle through. |

Fields
Collapse

## Usage

Useful for needing a way to cycle through references of any type.

## Examples

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ButtonReferenceCycle&oldid=90358](https://wiki.resonite.com/index.php?title=Component:ButtonReferenceCycle&oldid=90358)"

Contents