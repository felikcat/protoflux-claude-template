# Component:ReferenceEqualityDriver

> Source: https://wiki.resonite.com/Component:ReferenceEqualityDriver

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:ReferenceEqualityDriver&diff=92390) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/a/a7/ReferenceEqualityDriver%601Component.png/510px-ReferenceEqualityDriver%601Component.png)](https://wiki.resonite.com/File:ReferenceEqualityDriver%601Component.png) **Reference Equality Driver\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ReferenceEqualityDriver** component checks the equality of two objects and says whether they are equal. For objects that define their own behavior for checking Equality (Like Bounding boxes) this will check based on that logic (for Bounding boxes they only need to be numerically equal, like being the same size and center).

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `TargetReference` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [SyncRef\`1](https://wiki.resonite.com/Type:SyncRef%601 "Type:SyncRef`1") <T>>** | The reference to check. |
| `Reference` | **T** | The reference to use as a thing to compare against. |
| `Target` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | The boolean field to drive to whether `TargetReference` and `Reference` are equal. Doesn't always mean they are the exact same object. |
| `Invert` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to invert the result sent to `Target`. |

Fields
Collapse

## Usage

Attach to a slot and provide a reference object to check against, or provide nothing to check against if null or not null. Then put in a field to check for a reference inside of, and the component will start working.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Component:ValueEqualityDriver](https://wiki.resonite.com/Component:ValueEqualityDriver "Component:ValueEqualityDriver")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ReferenceEqualityDriver&oldid=92390](https://wiki.resonite.com/index.php?title=Component:ReferenceEqualityDriver&oldid=92390)"

Contents