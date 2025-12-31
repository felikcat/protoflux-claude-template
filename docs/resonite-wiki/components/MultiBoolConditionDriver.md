# Component:MultiBoolConditionDriver

> Source: https://wiki.resonite.com/Component:MultiBoolConditionDriver

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:MultiBoolConditionDriver&diff=113306) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/0/00/MultiBoolConditionDriverComponent.png/510px-MultiBoolConditionDriverComponent.png)](https://wiki.resonite.com/File:MultiBoolConditionDriverComponent.png) **MultiBoolConditionDriver** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **MultiBoolConditionDriver** drives `Target` depending on the state of the `Conditions` list, and the `ConditionMode` selected.

One popular use for this component is disabling meshes that need to be turned on or off in conjunction with other meshes.

For example, disabling fur tufts when clothing is enabled by using Active on each clothing item as a Condition, Mode set to 'None', and Target being Active on the fur tuft.

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Target` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | The field to drive to true if the bools in `Conditions` meet the conditions set by `ConditionMode` |
| `Mode` | **[MultiBoolConditionDriver.ConditionMode](https://wiki.resonite.com/Component:MultiBoolConditionDriver#ConditionMode)** | What state the bools in `Conditions` must be in, to drive `Target` to true. |
| `Conditions` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[MultiBoolConditionDriver.Condition](https://wiki.resonite.com/Component:MultiBoolConditionDriver#Condition)** | A list of bool fields to compare against the `ConditionMode` |

Fields
Collapse

## Behavior

Mode can be one of:

- All: Logical AND
- Any: Logical OR
- None: Logical NOR

## Examples

[![](https://wiki.resonite.com/images/thumb/0/00/MultiBoolConditionDriver_example1.png/300px-MultiBoolConditionDriver_example1.png)](https://wiki.resonite.com/File:MultiBoolConditionDriver_example1.png) Example showing normal and inverted inputs.

Top driven ValueField goes TRUE when the following conditions(Mode: All) are meet.

Condition 0 is TRUE

Condition 1 is TRUE

Condition 2 is FALSE (Due to 'invert' flag.)

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:MultiBoolConditionDriver&oldid=113306](https://wiki.resonite.com/index.php?title=Component:MultiBoolConditionDriver&oldid=113306)"

Contents