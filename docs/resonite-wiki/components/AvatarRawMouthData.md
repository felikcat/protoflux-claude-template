# Component:AvatarRawMouthData

> Source: https://wiki.resonite.com/Component:AvatarRawMouthData

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:AvatarRawMouthData&diff=95975) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/f/f6/AvatarRawMouthDataComponent.png/510px-AvatarRawMouthDataComponent.png)](https://wiki.resonite.com/File:AvatarRawMouthDataComponent.png) **Avatar Raw Mouth Data** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **AvatarRawMouthData** component reads the tracking values from any given `DataSource` and turns it into in game usable data.

This is useful for doing debugging or Debug on face or mouth tracking.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `DataSource` | **[IMouthTrackingSourceComponent](https://wiki.resonite.com/Type:IMouthTrackingSourceComponent "Type:IMouthTrackingSourceComponent")** | The place to get tracking data from. |
| `StrengthMultiplier` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to amplify the incoming data. |
| `Jaw` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The raw Jaw data from `DataSource` |
| `JawOpen` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The raw JawOpen data from `DataSource` |
| `Tongue` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The raw Tongue data from `DataSource` |
| `TongueRoll` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The raw TongueRoll data from `DataSource` |
| `LipUpperLeftRaise` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The raw LipUpperLeftRaise data from `DataSource` |
| `LipUpperRightRaise` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The raw LipUpperRightRaise data from `DataSource` |
| `LipLowerLeftRaise` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The raw LipLowerLeftRaise data from `DataSource` |
| `LipLowerRightRaise` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The raw LipLowerRightRaise data from `DataSource` |
| `LipUpperHorizontal` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The raw LipUpperHorizontal data from `DataSource` |
| `LipLowerHorizontal` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The raw LipLowerHorizontal data from `DataSource` |
| `MouthLeftSmileFrown` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The raw MouthLeftSmileFrown data from `DataSource` |
| `MouthRightSmileFrown` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The raw MouthRightSmileFrown data from `DataSource` |
| `MouthLeftDimple` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The raw MouthLeftDimple data from `DataSource` |
| `MouthRightDimple` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The raw MouthRightDimple data from `DataSource` |
| `MouthPout` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The raw MouthPout data from `DataSource` |
| `MouthPoutLeft` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The raw MouthPoutLeft data from `DataSource` |
| `MouthPoutRight` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The raw MouthPoutRight data from `DataSource` |
| `LipTopOverturn` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The raw LipTopOverturn data from `DataSource` |
| `LipTopLeftOverturn` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The raw LipTopLeftOverturn data from `DataSource` |
| `LipTopRightOverturn` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The raw LipTopRightOverturn data from `DataSource` |
| `LipBottomOverturn` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The raw LipBottomOverturn data from `DataSource` |
| `LipBottomLeftOverturn` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The raw LipBottomLeftOverturn data from `DataSource` |
| `LipBottomRightOverturn` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The raw LipBottomRightOverturn data from `DataSource` |
| `LipTopOverUnder` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The raw LipTopOverUnder data from `DataSource` |
| `LipTopLeftOverUnder` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The raw LipTopLeftOverUnder data from `DataSource` |
| `LipTopRightOverUnder` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The raw LipTopRightOverUnder data from `DataSource` |
| `LipBottomOverUnder` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The raw LipBottomOverUnder data from `DataSource` |
| `LipBottomLeftOverUnder` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The raw LipBottomLeftOverUnder data from `DataSource` |
| `LipBottomRightOverUnder` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The raw LipBottomRightOverUnder data from `DataSource` |
| `LipLeftStretchTighten` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The raw LipLeftStretchTighten data from `DataSource` |
| `LipRightStretchTighten` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The raw LipRightStretchTighten data from `DataSource` |
| `LipsLeftPress` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The raw LipsLeftPress data from `DataSource` |
| `LipsRightPress` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The raw LipsRightPress data from `DataSource` |
| `CheekLeftPuffSuck` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The raw CheekLeftPuffSuck data from `DataSource` |
| `CheekRightPuffSuck` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The raw CheekRightPuffSuck data from `DataSource` |
| `CheekLeftRaise` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The raw CheekLeftRaise data from `DataSource` |
| `CheekRightRaise` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The raw CheekRightRaise data from `DataSource` |
| `NoseWrinkleLeft` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The raw NoseWrinkleLeft data from `DataSource` |
| `NoseWrinkleRight` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The raw NoseWrinkleRight data from `DataSource` |
| `ChinRaiseBottom` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The raw ChinRaiseBottom data from `DataSource` |
| `ChinRaiseTop` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The raw ChinRaiseTop data from `DataSource` |

Fields
Collapse

## Usage

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AvatarRawMouthData&oldid=95975](https://wiki.resonite.com/index.php?title=Component:AvatarRawMouthData&oldid=95975)"

Contents