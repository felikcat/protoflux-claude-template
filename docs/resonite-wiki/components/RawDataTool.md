# Component:RawDataTool

> Source: https://wiki.resonite.com/Component:RawDataTool

Collapse **Component image**

[File:RawDataToolComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=RawDataToolComponent.png "File:RawDataToolComponent.png") **Raw Data Tool** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **RawDataTool** component is used in many different tool creations to allow for getting tool related actions on the hand its equipped in. This component has a ProtoFlux node associated with it ( [ProtoFlux:RawDataTool Events](https://wiki.resonite.com/ProtoFlux:RawDataTool_Events "ProtoFlux:RawDataTool Events"))

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `_equipLink` | _direct_ **[LinkTarget\`1](https://wiki.resonite.com/index.php?title=Type:LinkTarget%601&action=edit&redlink=1 "Type:LinkTarget`1 (page does not exist)") < [ITool](https://wiki.resonite.com/Type:ITool "Type:ITool") >** | This is Internal, and is used by the engine to retrieve the component this field is a part of. It cannot be assigned to. |
| `TipReference` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot to use as the tool's tip, instead of the component's slot. |
| `BlockGripEquip` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to prevent legacy double grip equipping from equipping this tooltip. |
| `BlockRemoteEquip` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to prevent equipping by clicking via laser |
| `EquipName` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The name of the tool in the context menu when equipping via context menu. |
| `_overrideActiveTool` | **[InteractionHandler](https://wiki.resonite.com/Component:InteractionHandler "Component:InteractionHandler")** | The interaction handler to use instead of this tool as an interaction handler. |
| `_gripPosesGenerated` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the [Grip Pose Reference](https://wiki.resonite.com/Component:GripPoseReference "Component:GripPoseReference") components and slots have been generated for this tool. |
| `LocalTipOffset` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | How much to offset the tool and its laser |
| `LocalTipReference` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot to use for the laser source and tip location. |
| `UseLaser` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to enable the use of and visual of the Laser. |
| `BlockPrimaryWhenTouching` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | blocks use of primary when the tool is touching a wall. |
| `UseSecondary` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Allow for use of secondary. When disabled on quest this disables the Tank Controls mode which many quest users in the resonite community dislike. |
| `AllowUseWhenHolding` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Allow use of the tool when the user is holding onto the tool rather than having it equipped. |
| `Equipped` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the tool is equipped or not. This will still return true if the user is holding onto the tip. Commonly referred to as "Soft Equipping" or "Pseudo Equipping". |
| `ControllerType` | _direct_ **[SyncType](https://wiki.resonite.com/Type:SyncType "Type:SyncType")** | The [Type](https://wiki.resonite.com/Type:Type "Type:Type") (C# class) of the controller holding this tool. |
| `ControllerSide` | **[Chirality](https://wiki.resonite.com/Type:Chirality "Type:Chirality")** | Whether the left, right, or none controller is holding this tool. |
| `PrimaryStrength` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The live updated value of the user's primary strength on this hand. Applies to VRcontrollers or game pad type controllers. |
| `SecondaryAxis` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The position of the thumb on the track pad used for secondary on this hand. |
| `Primary` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the user is pressing primary on this hand. See [Controls](https://wiki.resonite.com/Controls "Controls") |
| `Secondary` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the user is pressing secondary on this hand. See [Controls](https://wiki.resonite.com/Controls "Controls"). |
| `_primaryStrengthStream` | **[ValueStream\`1](https://wiki.resonite.com/index.php?title=Type:ValueStream%601&action=edit&redlink=1 "Type:ValueStream`1 (page does not exist)") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | The value stream of the primary strength value. This comes from a user's value streams which can be viewed through a [User Inspector](https://wiki.resonite.com/User_Inspector "User Inspector"). |
| `_secondaryAxisStream` | **[ValueStream\`1](https://wiki.resonite.com/index.php?title=Type:ValueStream%601&action=edit&redlink=1 "Type:ValueStream`1 (page does not exist)") < [Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2") >** | The value stream of the secondary strength value. This comes from a user's value streams which can be viewed through a [User Inspector](https://wiki.resonite.com/User_Inspector "User Inspector"). |
| `_primaryStream` | **[ValueStream\`1](https://wiki.resonite.com/index.php?title=Type:ValueStream%601&action=edit&redlink=1 "Type:ValueStream`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >** | The value stream of the primary pressed value. This comes from a user's value streams which can be viewed through a [User Inspector](https://wiki.resonite.com/User_Inspector "User Inspector"). |
| `_secondaryStream` | **[ValueStream\`1](https://wiki.resonite.com/index.php?title=Type:ValueStream%601&action=edit&redlink=1 "Type:ValueStream`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >** | The value stream of the secondary pressed value. This comes from a user's value streams which can be viewed through a [User Inspector](https://wiki.resonite.com/User_Inspector "User Inspector"). |
| `_rawStrength` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The Raw unfiltered value of the primary strength value. |
| `_rawAxis` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | the Raw unfiltered value of the secondary axis value. |
| `_rawPrimary` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | the Raw unfiltered value of the primary pressed value. |
| `_rawSecondary` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | the Raw unfiltered value of the secondary pressed value. |
| `PrimaryActionDescription` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | sets the label that tells the user what primary on this tool does. |
| `SecondaryActionDescription` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | sets the label that tells the user what secondary on this tool does. |

Fields
Collapse

## Usage

Attach to a slot and this component will generate the needed slots for this tool to work. This component will need a collider in its slot hierarchy so the tool can be grabbed and used. Combining this tool with protoflux or Components is needed to add custom behavior.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:RawDataTool&oldid=98657](https://wiki.resonite.com/index.php?title=Component:RawDataTool&oldid=98657)"

Contents