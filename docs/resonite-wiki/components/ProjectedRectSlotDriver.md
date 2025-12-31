# Component:ProjectedRectSlotDriver

> Source: https://wiki.resonite.com/Component:ProjectedRectSlotDriver

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:ProjectedRectSlotDriver&diff=88827) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/b/b6/ProjectedRectSlotDriverComponent.png/510px-ProjectedRectSlotDriverComponent.png)](https://wiki.resonite.com/File:ProjectedRectSlotDriverComponent.png) **ProjectedRectSlotDriver** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ProjectedRectSlotDriver** component takes a [Slot](https://wiki.resonite.com/Slot "Slot") in the `Target` field and places that slot in the center of where this compoennt's [UIX](https://wiki.resonite.com/UIX "UIX") element's transform is. This target slot will be resized to match a pizel scale that the UIX [Canvas](https://wiki.resonite.com/Component:Canvas "Component:Canvas") uses.

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `_position` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | Internal - The position of the target slot. |
| `Target` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot to reposition onto this UIX. |
| `_rotation` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | Internal - The rotation of the target slot. |
| `_scale` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | Internal - The scale of the target slot. |
| `_originalParent` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | Internal - The original parent this slot came from. |
| `_lastTarget` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | Internal - The last known slot target this component used. |

Fields
Collapse

## Usage

This can be used if you want to place a slot to where some [UIX](https://wiki.resonite.com/UIX "UIX") is at anytime.

## Examples

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ProjectedRectSlotDriver&oldid=88827](https://wiki.resonite.com/index.php?title=Component:ProjectedRectSlotDriver&oldid=88827)"

Contents