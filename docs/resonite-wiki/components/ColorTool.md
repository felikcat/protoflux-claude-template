# Component:ColorTool

> Source: https://wiki.resonite.com/Component:ColorTool

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/b/b5/ColorToolComponent.png/510px-ColorToolComponent.png)](https://wiki.resonite.com/File:ColorToolComponent.png) **Color Tool** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

Color tool is a component that drives the color tool from [Tools](https://wiki.resonite.com/Tools "Tools"). Pressing [Secondary](https://wiki.resonite.com/Controls "Controls") allows for picking a color via raycast, and hitting [Primary](https://wiki.resonite.com/Controls "Controls") allows for setting the color of a material.

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
| `Color` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The selected color for this tool. |
| `EnsureUniqueMaterial` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Creates a new material rather than changing the color of the material of a target object when hitting [Primary](https://wiki.resonite.com/Controls "Controls"). |
| `ColorIndicators` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[FieldDrive\`1](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1") < [ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX") >** | The field to drive to the current picked color. used for an indicator. |
| `_colorDialog` | _direct_ **[SlotCleanupRef\`1](https://wiki.resonite.com/index.php?title=Type:SlotCleanupRef%601&action=edit&redlink=1 "Type:SlotCleanupRef`1 (page does not exist)") < [ColorDialogInterface](https://wiki.resonite.com/Component:ColorDialogInterface "Component:ColorDialogInterface") >** | The currently open color picker dialogue. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `OpenColorDialog:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Handles spawning the user's favorite color picker so they can edit this tool's color. |

Triggers
Collapse

## Behavior

## Examples

Can be used to pick colors from surfaces, or it can be used to quickly color objects.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ColorTool&oldid=98347](https://wiki.resonite.com/index.php?title=Component:ColorTool&oldid=98347)"

Contents