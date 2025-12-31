# Component:ScaleAligner

> Source: https://wiki.resonite.com/Component:ScaleAligner

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:ScaleAligner&diff=113557) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/0/06/ScaleAlignerComponent.png/510px-ScaleAlignerComponent.png)](https://wiki.resonite.com/File:ScaleAlignerComponent.png) **Scale Aligner** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ScaleAligner** component scales a list of slots based on bounding box, each one being bigger/smaller than the last.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `AutoAddChildren` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether slots below this component's slot in the hierarchy are automatically added to `_targets` |
| `AutoAddIgnoreTags` | _direct_ **[SyncFieldList\`1](https://wiki.resonite.com/Type:SyncFieldList%601 "Type:SyncFieldList`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | _This article or section is a stub. You can help the Resonite wiki by expanding it._ |
| `BaseSize` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The size the first item should be in local space based on Bounding box. |
| `Increment` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | How much to make the next item in the list bigger/smaller than the last by adding to its Bounding box size. |
| `Multiplier` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | How much to make the next item in the list bigger/smaller than the last by multiplying its Bounding box size after adding `Increment` |
| `NonUniform` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether scaling can be non uniform for Bounding box Scale calculations. |
| `_targets` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[ScaleAligner.Target](https://wiki.resonite.com/Component:ScaleAligner#Target)** | A list of slots and their scales to influence. |

Fields
Collapse

## Target

| Name | Type | Description |
| --- | --- | --- |
| `TargetSlot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot this Target entry is targeting. |
| `ScaleDrive` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The scale field of `TargetSlot`. |

Fields

## Usage

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ScaleAligner&oldid=113557](https://wiki.resonite.com/index.php?title=Component:ScaleAligner&oldid=113557)"

Contents