# Component:ObjectScroller

> Source: https://wiki.resonite.com/Component:ObjectScroller

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:ObjectScroller&diff=97647) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/f/f2/ObjectScrollerComponent.png/510px-ObjectScrollerComponent.png)](https://wiki.resonite.com/File:ObjectScrollerComponent.png) **Object Scroller** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ObjectScroller** component acts as a way to scroll a list of items with sizes by offsetting them within a region they should appear within. Objects outside of the region get disabled until the `Offset` allows them to appear within it again.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Items` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[ObjectScroller.Item](https://wiki.resonite.com/Component:ObjectScroller#Item)** | A list of items to move and activate/deactivate if they are within/outside of the `RegionSize` |
| `Offset` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | How much to offset the positions of `Items` in order to scroll them. |
| `RegionSize` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The size area objects have to be touching from their current position and size after `Offset` is applied in order to stay visible. |

Fields
Collapse

## Item

| Name | Type | Description |
| --- | --- | --- |
| `Position` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | Original position of the item before `Offset`. |
| `Size` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The size of this item. |
| `PositionDrive` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | Drives the item's position so `Offset` can affect it. |
| `ScaleDrive` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | Used to scale the item down if the item cannot fit within `RegionSize` at its current position. |
| `ActiveDrive` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Used to enable/disable the item if it's inside/outside of `RegionSize`. |

Fields

## Usage

Attach to a slot and add/setup `Items` entries to begin use.

## Examples

Can be used to make a conveyor belt of items or a sliding wardrobe of avatars.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ObjectScroller&oldid=97647](https://wiki.resonite.com/index.php?title=Component:ObjectScroller&oldid=97647)"

Contents