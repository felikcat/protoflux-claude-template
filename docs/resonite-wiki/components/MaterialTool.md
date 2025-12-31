# Component:MaterialTool

> Source: https://wiki.resonite.com/Component:MaterialTool

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/b/b4/MaterialToolComponent.png/510px-MaterialToolComponent.png)](https://wiki.resonite.com/File:MaterialToolComponent.png) **Material Tool** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

See [Material Tool](https://wiki.resonite.com/Material_Tool "Material Tool").

## Usage

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
| `_orbSlot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot to store the material orb when an orb is placed into the tool or picked from an object. |
| `ReplacementMode` | **[AssetToolReplacementMode](https://wiki.resonite.com/Type:AssetToolReplacementMode "Type:AssetToolReplacementMode")** | How to replace materials using the tool. |
| `AreaRadius` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The radius to use when `ReplacementMode` is set to Area. |
| `_areaIndicator` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot that is the root of the area indicator visual. |
| `_areaIndicatorRadius` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The area indicator's radius field. |
| `_areaIndicatorOffset` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The area indicator's offset field. |
| `_areaIndicatorActive` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | The area indicator's active field, used to disable the visual when `ReplacementMode` is not set to Area. |
| `_knobControlActive` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | The active field of the knob control visual/control. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| ``SnapFilter:Func`3<Snapper, SnapTarget, Bool>`` | **[Func\`3](https://wiki.resonite.com/Type:Func%603 "Type:Func`3") < [Snapper](https://wiki.resonite.com/Component:Snapper "Component:Snapper"), [SnapTarget](https://wiki.resonite.com/Component:SnapTarget "Component:SnapTarget"), [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >** | ✓ | A function that can be used in a snapper to filter what objects can snap to a snapper (filters to material orbs only). |
| `EditMaterial:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the edit material button is touched. |
| `CreateCopy:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the create copy button is touched. |
| `CreateMaterial:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the create material button is touched. |
| ``ConvertAllMaterials:ButtonEventHandler`1<Slot>`` | **[ButtonEventHandler\`1](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler%601&action=edit&redlink=1 "Type:ButtonEventHandler`1 (page does not exist)") < [Slot](https://wiki.resonite.com/Type:Slot "Type:Slot") >** | ✓ | Called when the convert all button is touched. |
| `ConvertMaterial:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the convert button is touched. |
| ``RunConversion:Action`2<DevCreateNewForm, Slot>`` | **[Action\`2](https://wiki.resonite.com/index.php?title=Type:Action%602&action=edit&redlink=1 "Type:Action`2 (page does not exist)") < [DevCreateNewForm](https://wiki.resonite.com/Component:DevCreateNewForm "Component:DevCreateNewForm"), [Slot](https://wiki.resonite.com/Type:Slot "Type:Slot") >** | ✓ | Called when the convert process is started. |
| `CanKnobControlInteract:GrabCheck` | **[GrabCheck](https://wiki.resonite.com/Type:GrabCheck "Type:GrabCheck")** | ✓ | Can be used to check if a grabber is allowed to interact with a grabber. **Can be used to filter the same hand from grabbing an item on this material tip! (possibly only instance of this behavior being possible)** |

Triggers
Collapse

## Usage

See [Material Tool](https://wiki.resonite.com/Material_Tool "Material Tool").

## Examples

See [Material Tool](https://wiki.resonite.com/Material_Tool "Material Tool").

## See Also

- [Material Tool](https://wiki.resonite.com/Material_Tool "Material Tool")
- [Tools](https://wiki.resonite.com/Tools "Tools")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:MaterialTool&oldid=99070](https://wiki.resonite.com/index.php?title=Component:MaterialTool&oldid=99070)"

Contents