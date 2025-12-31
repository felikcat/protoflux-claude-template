# Component:MockupMouthTrackingSource

> Source: https://wiki.resonite.com/Component:MockupMouthTrackingSource

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/4/46/MockupMouthTrackingSourceComponent.png/510px-MockupMouthTrackingSourceComponent.png)](https://wiki.resonite.com/File:MockupMouthTrackingSourceComponent.png) **Mockup Mouth Tracking Source** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **MockupMouthTrackingSource** component can be used to simulate the tracking data of a tracking device and be applied to any field that takes a [IMouthTrackingSourceComponent](https://wiki.resonite.com/Type:IMouthTrackingSourceComponent "Type:IMouthTrackingSourceComponent").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Jaw` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The jaw position from rest. |
| `JawOpen` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The jaw openess. |
| `Tongue` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The tongue position. |
| `TongueRoll` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The tongue roll into a burrito shape. |
| `LipUpperLeftRaise` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The upper left lip raise amount. |
| `LipUpperRightRaise` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The upper right lip raise amount. |
| `LipLowerLeftRaise` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The lower left lip raise amount. |
| `LipLowerRightRaise` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The lower right lip raise amount. |
| `LipUpperHorizontal` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The shift side to side of the upper lip. |
| `LipLowerHorizontal` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The shift side to side of the lower lip. (negative to positive 1) |
| `MouthLeftSmileFrown` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The left frown/smile amount. (negative to positive 1) |
| `MouthRightSmileFrown` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The right frown/smile amount. (negative to positive 1) |
| `MouthLeftDimple` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | push the area closest to the corners of the lips inwards on the left. |
| `MouthRightDimple` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | push the area closest to the corners of the lips inwards on the right. |
| `MouthPoutLeft` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The mouth kissy amount on the left. |
| `MouthPoutRight` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The mouth kissy amount on the right. |
| `LipTopLeftOverturn` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The amount The top lip is flipping upwards on the left. |
| `LipTopRightOverturn` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The amount The top lip is flipping upwards on the right. |
| `LipBottomLeftOverturn` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The amount The top lip is flipping upwards |
| `LipBottomRightOverturn` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | how much the bottom right side of the lips is pushing outwards like duck lips. |
| `LipTopLeftOverUnder` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The amount the top lip is going down to cover the bottom lip. |
| `LipTopRightOverUnder` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much the bottom right part of the lips is going behind the top right lip. |
| `LipBottomLeftOverUnder` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The amount the bottom lip is going up to cover the top lip left. |
| `LipBottomRightOverUnder` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The amount the bottom lip is going up to cover the top lip right. |
| `LipLeftStretchTighten` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The amount the left side of the lips are pulling towards the outside. |
| `LipRightStretchTighten` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The amount the right side of the lips are pulling towards the outside. |
| `LipsLeftPress` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The amount the left side of the lips are pulling towards the inside. |
| `LipsRightPress` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The amount the right side of the lips are pulling towards the inside. |
| `CheekLeftPuffSuck` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The amount the left cheek is sucking inwards or being puffed out. (negative to positive 1) |
| `CheekRightPuffSuck` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The amount the right cheek is sucking inwards or being puffed out. (negative to positive 1) |
| `CheekLeftRaise` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much the cheek area of the left side of the face is being pushed upwards (Usually caused by smile) (negative to positive one) |
| `CheekRightRaise` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much the cheek area of the right side of the face is being pushed upwards (Usually caused by smile) (negative to positive one) |
| `NoseWrinkleLeft` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much the left side of the nose is being pushed up. |
| `NoseWrinkleRight` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much the right side of the nose is being pushed up. |
| `ChinRaiseBottom` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much the bottom chin is being pulled up. |
| `ChinRaiseTop` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much the top chin is being pulled up. |

Fields
Collapse

## Usage

Attach to a slot and insert the component into another Component on an avatar like an [Component:AvatarExpressionDriver](https://wiki.resonite.com/Component:AvatarExpressionDriver "Component:AvatarExpressionDriver") to test its value influences.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:MockupMouthTrackingSource&oldid=105334](https://wiki.resonite.com/index.php?title=Component:MockupMouthTrackingSource&oldid=105334)"

Contents