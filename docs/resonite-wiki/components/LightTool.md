# Component:LightTool

> Source: https://wiki.resonite.com/Component:LightTool

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/a/a8/LightToolComponent.png/510px-LightToolComponent.png)](https://wiki.resonite.com/File:LightToolComponent.png) **Light Tool** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **LightTool** component can be best learned through its page, the [Light Tool](https://wiki.resonite.com/Light_Tool "Light Tool") for non power users.

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
| `LightMode` | **[LightTool.Mode](https://wiki.resonite.com/Component:LightTool#Mode)** | See [Mode](https://wiki.resonite.com/Component:LightTool#Mode). |
| `Color` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color to make new lights. |
| `Intensity` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The intensity to make new lights. |
| `ShadowType` | **[ShadowType](https://wiki.resonite.com/Type:ShadowType "Type:ShadowType")** | The shadow type to make new lights. |
| `ShadowStrength` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The strength for the shadows new lights should have. |
| `Range` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The range of new lights. |
| `SpotAngle` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The spot angle of new lights. |
| `PointLightVisual` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The current point light visual root. |
| `SpotlightVisual` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The current spot light visual root. |
| `DirectionalLightVisual` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The current directional light visual root. |
| `ColorIndicators` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[FieldDrive\`1](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1") < [ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX") >** | A list of color fields to drive with the indication color. |
| `ShowGizmo` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to show the Gizmo of new lights. |
| `_pointLightItem` | **[LegacySegmentCircleMenuController.Item](https://wiki.resonite.com/Component:LegacySegmentCircleMenuController#Item "Component:LegacySegmentCircleMenuController")** | Legacy don't use. |
| `_spotLightItem` | **[LegacySegmentCircleMenuController.Item](https://wiki.resonite.com/Component:LegacySegmentCircleMenuController#Item "Component:LegacySegmentCircleMenuController")** | Legacy don't use. |
| `_directionalLightItem` | **[LegacySegmentCircleMenuController.Item](https://wiki.resonite.com/Component:LegacySegmentCircleMenuController#Item "Component:LegacySegmentCircleMenuController")** | Legacy don't use. |
| `_shadowsItem` | **[LegacySegmentCircleMenuController.Item](https://wiki.resonite.com/Component:LegacySegmentCircleMenuController#Item "Component:LegacySegmentCircleMenuController")** | Legacy don't use. |
| `_colorPicker` | _direct_ **[SlotCleanupRef\`1](https://wiki.resonite.com/index.php?title=Type:SlotCleanupRef%601&action=edit&redlink=1 "Type:SlotCleanupRef`1 (page does not exist)") < [ColorDialogInterface](https://wiki.resonite.com/Component:ColorDialogInterface "Component:ColorDialogInterface") >** | The current color picker being used to pick the color for `Color`. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `OnChangeColor:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Handles when the user clicks the menu option to change the created light color. |

Triggers
Collapse

## Mode

| Name | Value | Description |
| --- | --- | --- |
| `PointLight` | 0 | Point light mode will let you create point light orbs by clicking primary. |
| `Spotlight` | 1 | Spot will allow you to create spot light cones by clicking primary. |
| `MoveSun` | 2 | Sun will allow you to move the sun to where you are currently clicking in the sky. |

Values

## Usage

See [Light Tool](https://wiki.resonite.com/Light_Tool "Light Tool").

## See Also

- [Light Tool](https://wiki.resonite.com/Light_Tool "Light Tool")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:LightTool&oldid=98972](https://wiki.resonite.com/index.php?title=Component:LightTool&oldid=98972)"

Contents