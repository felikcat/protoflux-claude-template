# Component:RectSlotDriver

> Source: https://wiki.resonite.com/Component:RectSlotDriver

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:RectSlotDriver&diff=88830) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/2/23/RectSlotDriverComponent.png/510px-RectSlotDriverComponent.png)](https://wiki.resonite.com/File:RectSlotDriverComponent.png) **RectSlotDriver** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **RectSlotDriver** component, when attached to a [UIX](https://wiki.resonite.com/UIX "UIX") element [slot](https://wiki.resonite.com/Slot "Slot"), will automatically drive that slot's position and will provide a field `_position` for the [user](https://wiki.resonite.com/User "User") to use as a reference.

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `_position` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | Internal - Sets the position of the slot for driving the value. |

Fields
Collapse

## Usage

Mostly will be used for reference of a position of a [UIX](https://wiki.resonite.com/UIX "UIX") element.

## Examples

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:RectSlotDriver&oldid=88830](https://wiki.resonite.com/index.php?title=Component:RectSlotDriver&oldid=88830)"

Contents