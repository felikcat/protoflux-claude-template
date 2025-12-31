# Component:ValueEqualityDriver

> Source: https://wiki.resonite.com/Component:ValueEqualityDriver

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:ValueEqualityDriver&diff=92391) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/d/db/ValueEqualityDriver%601Component.png/510px-ValueEqualityDriver%601Component.png)](https://wiki.resonite.com/File:ValueEqualityDriver%601Component.png) **Value Equality Driver\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ValueEqualityDriver** component lets you drive a boolean to whether or not one value is equal to another.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `TargetValue` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") <T>>** | The value being compared to `Reference`. |
| `Reference` | **T** | The value that `TargetValue` is being compared to. |
| `Target` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | The boolean that is driven to true if `TargetValue` is equal to `Reference` and false if it isn't. |
| `Invert` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to invert the result of `TargetValue` |
| `UseApproximateComparison` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether or not to use approximate comparison for types such as float, where values that seem identical can be very slightly different. |

Fields
Collapse

## Usage

Use to drive the target boolean with whether the target's value is equal to the reference value.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Component:ReferenceEqualityDriver](https://wiki.resonite.com/Component:ReferenceEqualityDriver "Component:ReferenceEqualityDriver")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ValueEqualityDriver&oldid=92391](https://wiki.resonite.com/index.php?title=Component:ValueEqualityDriver&oldid=92391)"

Contents