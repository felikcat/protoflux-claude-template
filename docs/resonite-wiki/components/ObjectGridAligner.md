# Component:ObjectGridAligner

> Source: https://wiki.resonite.com/Component:ObjectGridAligner

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:ObjectGridAligner&diff=105347) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/6/65/ObjectGridAlignerComponent.png/510px-ObjectGridAlignerComponent.png)](https://wiki.resonite.com/File:ObjectGridAlignerComponent.png) **Object Grid Aligner** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ObjectGridAligner** component aligns objects into a grid of items with x number of items per row.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `AutoAddChildren` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether slots below this component's slot in the hierarchy are automatically added to `_targets`. |
| `AutoAddIgnoreTags` | _direct_ **[SyncFieldList\`1](https://wiki.resonite.com/Type:SyncFieldList%601 "Type:SyncFieldList`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | Slots that have these tags are automatically ignored by this component when adding children slots. |
| `ItemsPerRow` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | How many items per row. |
| `CellSize` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The space between each item. |
| `LerpSpeed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How fast the items should move to align themselves in the specified grid arrangement. |
| `HorizontalAlignment` | **[ObjectGridAligner.Align](https://wiki.resonite.com/Component:ObjectGridAligner#Align)** | How to align the items horizontally. |
| `VerticalAlignment` | **[ObjectGridAligner.Align](https://wiki.resonite.com/Component:ObjectGridAligner#Align)** | How to align the items vertically. |
| `RowAxis` | **[ObjectGridAligner.AxisDir](https://wiki.resonite.com/Component:ObjectGridAligner#AxisDir)** | The axis that items should be aligned on for the horizontal axis of the grid. |
| `ColumnAxis` | **[ObjectGridAligner.AxisDir](https://wiki.resonite.com/Component:ObjectGridAligner#AxisDir)** | The axis that items should be aligned on for the vertical axis of the grid. |
| `Items` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[ObjectGridAligner.Item](https://wiki.resonite.com/Component:ObjectGridAligner#Item)** | A list of items who's positions should be driven to place them into a grid alignment using this component's calculations. |

Fields
Collapse

## Align

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Controls how the items should align themselves along the axis specified by the component.

| Name | Value | Description |
| --- | --- | --- |
| `Neg` | 0 | Aligns items so their values are always negative along the specified alignment axis (so if using x axis, x will always be negative for an item) |
| `Mid` | 1 | Aligns items so half are on the negative and half are on the positive along an axis, so they take up both directions equally. |
| `Pos` | 2 | Aligns items so their values are always positive along the specified alignment axis (so if using x axis, x will always be positive for an item) |

Values

## AxisDir

_This article or section is a stub. You can help the Resonite wiki by expanding it._

| Name | Value | Description |
| --- | --- | --- |
| `Xpos` | 0 | Align items along the positive x axis. |
| `Xneg` | 1 | Align items along the negative x axis. |
| `Ypos` | 2 | Align items along the positive y axis. |
| `Yneg` | 3 | Align items along the negative y axis. |
| `Zpos` | 4 | Align items along the positive z axis. |
| `Zneg` | 5 | Align items along the negative z axis. |

Values

## Item

| Name | Type | Description |
| --- | --- | --- |
| `Root` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot to align. |
| `PositionDrive` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The position field of `Root`. |

Fields

## Usage

Can be used for aligning tiles, shelves, boxes, or anything that needs consistent alignment.

## Examples

- [ObjectGridAligner tutorial](https://www.youtube.com/watch?v=d4ouwoLrrho) by [ProbablePrime](https://wiki.resonite.com/User:ProbablePrime "User:ProbablePrime")

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ObjectGridAligner&oldid=105347](https://wiki.resonite.com/index.php?title=Component:ObjectGridAligner&oldid=105347)"

Contents