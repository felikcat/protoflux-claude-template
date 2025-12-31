# Component:MouthTrackingStreamManager

> Source: https://wiki.resonite.com/Component:MouthTrackingStreamManager

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:MouthTrackingStreamManager&diff=105338) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/2/21/MouthTrackingStreamManagerComponent.png/510px-MouthTrackingStreamManagerComponent.png)](https://wiki.resonite.com/File:MouthTrackingStreamManagerComponent.png) **MouthTrackingStreamManager** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **MouthTrackingStreamManager** component uses streaming data from the [ValueStream](https://wiki.resonite.com/index.php?title=Component:ValueStream&action=edit&redlink=1 "Component:ValueStream (page does not exist)") component (seen in the [user Inspector](https://wiki.resonite.com/User_Inspector "User Inspector")) to control the mouth on a [user's](https://wiki.resonite.com/User "User") [avatar](https://wiki.resonite.com/Avatar "Avatar").

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `User` | **[User](https://wiki.resonite.com/Type:User "Type:User")** | The referenced user to get the streamed data. |
| `IsTracking` | **[ValueStream\`1](https://wiki.resonite.com/index.php?title=Type:ValueStream%601&action=edit&redlink=1 "Type:ValueStream`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >** | Should we track the mouth. |
| `Jaw` | **[ValueStream\`1](https://wiki.resonite.com/index.php?title=Type:ValueStream%601&action=edit&redlink=1 "Type:ValueStream`1 (page does not exist)") < [Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3") >** | The streamed data for the Jaw. |
| `JawOpen` | **[ValueStream\`1](https://wiki.resonite.com/index.php?title=Type:ValueStream%601&action=edit&redlink=1 "Type:ValueStream`1 (page does not exist)") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | The streamed data for the Jaw opening. |
| `Tongue` | **[ValueStream\`1](https://wiki.resonite.com/index.php?title=Type:ValueStream%601&action=edit&redlink=1 "Type:ValueStream`1 (page does not exist)") < [Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3") >** | The streamed data for the tongue. |
| `TongueRoll` | **[ValueStream\`1](https://wiki.resonite.com/index.php?title=Type:ValueStream%601&action=edit&redlink=1 "Type:ValueStream`1 (page does not exist)") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | The streamed data for the tongue rolling. |
| `LipUpperLeftRaise` | **[ValueStream\`1](https://wiki.resonite.com/index.php?title=Type:ValueStream%601&action=edit&redlink=1 "Type:ValueStream`1 (page does not exist)") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | The streamed data for the lip (upper-left raised). |
| `LipUpperRightRaise` | **[ValueStream\`1](https://wiki.resonite.com/index.php?title=Type:ValueStream%601&action=edit&redlink=1 "Type:ValueStream`1 (page does not exist)") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | The streamed data for the lip (upper-right raised). |
| `LipLowerLeftaise` | **[ValueStream\`1](https://wiki.resonite.com/index.php?title=Type:ValueStream%601&action=edit&redlink=1 "Type:ValueStream`1 (page does not exist)") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | The streamed data for the lip (lower-left raised). |
| `LipLowerRightRaise` | **[ValueStream\`1](https://wiki.resonite.com/index.php?title=Type:ValueStream%601&action=edit&redlink=1 "Type:ValueStream`1 (page does not exist)") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | The streamed data for the lip (lower-right raised). |
| `LipUpperHorizontal` | **[ValueStream\`1](https://wiki.resonite.com/index.php?title=Type:ValueStream%601&action=edit&redlink=1 "Type:ValueStream`1 (page does not exist)") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | The streamed data for the lip (upper-horizontal). |
| `LipLowerHorizontal` | **[ValueStream\`1](https://wiki.resonite.com/index.php?title=Type:ValueStream%601&action=edit&redlink=1 "Type:ValueStream`1 (page does not exist)") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | The streamed data for the lip (lower-horizontal). |
| `MouthLeftSmileFrown` | **[ValueStream\`1](https://wiki.resonite.com/index.php?title=Type:ValueStream%601&action=edit&redlink=1 "Type:ValueStream`1 (page does not exist)") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | The streamed data for the mouth (left frown). |
| `MouthRightSmileFrown` | **[ValueStream\`1](https://wiki.resonite.com/index.php?title=Type:ValueStream%601&action=edit&redlink=1 "Type:ValueStream`1 (page does not exist)") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | The streamed data for the mouth (right frown). |
| `MouthLeftDimple` | **[ValueStream\`1](https://wiki.resonite.com/index.php?title=Type:ValueStream%601&action=edit&redlink=1 "Type:ValueStream`1 (page does not exist)") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | The stream for pushing the area closest to the corners of the lips inwards on the left. |
| `MouthRightDimple` | **[ValueStream\`1](https://wiki.resonite.com/index.php?title=Type:ValueStream%601&action=edit&redlink=1 "Type:ValueStream`1 (page does not exist)") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | The stream for pushing the area closest to the corners of the lips inwards on the right. |
| `MouthPoutLeft` | **[ValueStream\`1](https://wiki.resonite.com/index.php?title=Type:ValueStream%601&action=edit&redlink=1 "Type:ValueStream`1 (page does not exist)") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | The stream for the mouth kissy amount on the left. |
| `MouthPoutRight` | **[ValueStream\`1](https://wiki.resonite.com/index.php?title=Type:ValueStream%601&action=edit&redlink=1 "Type:ValueStream`1 (page does not exist)") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | The stream for the mouth kissy amount on the right. |
| `LipTopLeftOverturn` | **[ValueStream\`1](https://wiki.resonite.com/index.php?title=Type:ValueStream%601&action=edit&redlink=1 "Type:ValueStream`1 (page does not exist)") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | The stream for the amount The top lip is flipping outwards on the left. |
| `LipTopRightOverturn` | **[ValueStream\`1](https://wiki.resonite.com/index.php?title=Type:ValueStream%601&action=edit&redlink=1 "Type:ValueStream`1 (page does not exist)") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | The stream for the amount The top lip is flipping outwards on the right. |
| `LipBottomLeftOverturn` | **[ValueStream\`1](https://wiki.resonite.com/index.php?title=Type:ValueStream%601&action=edit&redlink=1 "Type:ValueStream`1 (page does not exist)") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | The stream for the amount The bottom lip is flipping outwards on the left. |
| `LipBottomRightOverturn` | **[ValueStream\`1](https://wiki.resonite.com/index.php?title=Type:ValueStream%601&action=edit&redlink=1 "Type:ValueStream`1 (page does not exist)") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | The stream for The amount The bottom lip is flipping outwards on the right. |
| `LipTopLeftOverUnder` | **[ValueStream\`1](https://wiki.resonite.com/index.php?title=Type:ValueStream%601&action=edit&redlink=1 "Type:ValueStream`1 (page does not exist)") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | The stream for the amount the top lip is going up to cover the bottom lip left. |
| `LipTopRightOverUnder` | **[ValueStream\`1](https://wiki.resonite.com/index.php?title=Type:ValueStream%601&action=edit&redlink=1 "Type:ValueStream`1 (page does not exist)") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | The stream for the amount the top lip is going up to cover the bottom lip right. |
| `LipBottomLeftOverUnder` | **[ValueStream\`1](https://wiki.resonite.com/index.php?title=Type:ValueStream%601&action=edit&redlink=1 "Type:ValueStream`1 (page does not exist)") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | The stream for the amount the bottom lip is going up to cover the top lip left. |
| `LipBottomRightOverUnder` | **[ValueStream\`1](https://wiki.resonite.com/index.php?title=Type:ValueStream%601&action=edit&redlink=1 "Type:ValueStream`1 (page does not exist)") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | The stream for the amount the bottom lip is going up to cover the top lip right. |
| `LipLeftStretchTighten` | **[ValueStream\`1](https://wiki.resonite.com/index.php?title=Type:ValueStream%601&action=edit&redlink=1 "Type:ValueStream`1 (page does not exist)") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | The stream for the amount the left side of the lips are pulling towards the outside. |
| `LipRightStretchTighten` | **[ValueStream\`1](https://wiki.resonite.com/index.php?title=Type:ValueStream%601&action=edit&redlink=1 "Type:ValueStream`1 (page does not exist)") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | The stream for the amount the right side of the lips are pulling towards the outside. |
| `LipsLeftPress` | **[ValueStream\`1](https://wiki.resonite.com/index.php?title=Type:ValueStream%601&action=edit&redlink=1 "Type:ValueStream`1 (page does not exist)") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | The stream for the amount the left side of the lips are pulling towards the inside. |
| `LipsRightPress` | **[ValueStream\`1](https://wiki.resonite.com/index.php?title=Type:ValueStream%601&action=edit&redlink=1 "Type:ValueStream`1 (page does not exist)") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | The stream for the amount the right side of the lips are pulling towards the inside. |
| `CheekLeftPuffSuck` | **[ValueStream\`1](https://wiki.resonite.com/index.php?title=Type:ValueStream%601&action=edit&redlink=1 "Type:ValueStream`1 (page does not exist)") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | The streamed data for the cheek (left puff). |
| `CheekRightPuffSuck` | **[ValueStream\`1](https://wiki.resonite.com/index.php?title=Type:ValueStream%601&action=edit&redlink=1 "Type:ValueStream`1 (page does not exist)") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | The streamed data for the cheek (right puff). |
| `CheekLeftRaise` | **[ValueStream\`1](https://wiki.resonite.com/index.php?title=Type:ValueStream%601&action=edit&redlink=1 "Type:ValueStream`1 (page does not exist)") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | The stream for how much the cheek area of the left side of the face is being pushed upwards (Usually caused by smile) (negative to positive one) |
| `CheekRightRaise` | **[ValueStream\`1](https://wiki.resonite.com/index.php?title=Type:ValueStream%601&action=edit&redlink=1 "Type:ValueStream`1 (page does not exist)") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | The stream for how much the cheek area of the right side of the face is being pushed upwards (Usually caused by smile) (negative to positive one) |
| `NoseWrinkleLeft` | **[ValueStream\`1](https://wiki.resonite.com/index.php?title=Type:ValueStream%601&action=edit&redlink=1 "Type:ValueStream`1 (page does not exist)") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | The stream for how much the left side of the nose is being pushed up. |
| `NoseWrinkleRight` | **[ValueStream\`1](https://wiki.resonite.com/index.php?title=Type:ValueStream%601&action=edit&redlink=1 "Type:ValueStream`1 (page does not exist)") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | The stream for how much the right side of the nose is being pushed up. |
| `ChinRaiseBottom` | **[ValueStream\`1](https://wiki.resonite.com/index.php?title=Type:ValueStream%601&action=edit&redlink=1 "Type:ValueStream`1 (page does not exist)") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | The stream for how much the bottom chin is being pulled up. |
| `ChinRaiseTop` | **[ValueStream\`1](https://wiki.resonite.com/index.php?title=Type:ValueStream%601&action=edit&redlink=1 "Type:ValueStream`1 (page does not exist)") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | The stream for how much the top chin is being pulled up. |

Fields
Collapse

## Usage

Used for [Mouth Tracking](https://wiki.resonite.com/index.php?title=Mouth_Tracking&action=edit&redlink=1 "Mouth Tracking (page does not exist)") internally.

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:MouthTrackingStreamManager&oldid=105338](https://wiki.resonite.com/index.php?title=Component:MouthTrackingStreamManager&oldid=105338)"

Contents