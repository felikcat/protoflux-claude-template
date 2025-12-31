# Component:DistanceMeter

> Source: https://wiki.resonite.com/Component:DistanceMeter

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/9/9f/DistanceMeterComponent.png/510px-DistanceMeterComponent.png)](https://wiki.resonite.com/File:DistanceMeterComponent.png) **Distance Meter** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **DistanceMeter** component is used by the [Meter Tool](https://wiki.resonite.com/Meter_Tool "Meter Tool") to display the distance between slots placed by it.

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Anchors` | _[list](https://wiki.resonite.com/Type:SyncRefList%601 "Type:SyncRefList`1")_ of **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | List of points being used to measure right now. |
| `_legacyAnchor0` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | Legacy, unused. For when the tool only measured two points. |
| `_legacyAnchor1` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | Legacy, unused. For when the tool only measured two points. |
| `FormatUnit` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The formatting string to use when formatting the distance number |
| `FormatNumber` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | How to format the distance number |
| `CompoundFormatUnits` | _direct_ **[SyncFieldList\`1](https://wiki.resonite.com/Type:SyncFieldList%601 "Type:SyncFieldList`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | The format string to format compound measurement units with. |
| `CompoundUseLongNames` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to use long name of distance (Ex: cm vs Centimeter) |
| `CompoundOverrideNames` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to use compound measurements or not. |
| `CompoundDiscardLastFraction` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to discard small distances like Millimeters. |
| `CompoundSeparator` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | What to separate compound measurements with (like spaces or commas) |
| `CompoundZeroHandling` | **[CompoundZeroHandling](https://wiki.resonite.com/Type:CompoundZeroHandling "Type:CompoundZeroHandling")** | How to handle compound measurements (1 meter 1cm 10mm) |
| `MeasurementSpace` | _direct_ **[RootSpace](https://wiki.resonite.com/Type:RootSpace "Type:RootSpace")** | The transform space to measure in. |
| `DistanceText` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | The field to drive when displaying the total amount of distance. |

Fields
Collapse

## Usage

See [Meter Tool](https://wiki.resonite.com/Meter_Tool "Meter Tool").

## Examples

See [Meter Tool](https://wiki.resonite.com/Meter_Tool "Meter Tool").

## See Also

- [Meter Tool](https://wiki.resonite.com/Meter_Tool "Meter Tool")
- [Tools](https://wiki.resonite.com/Tools "Tools")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:DistanceMeter&oldid=93773](https://wiki.resonite.com/index.php?title=Component:DistanceMeter&oldid=93773)"

Contents