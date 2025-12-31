# Component:GlueTool

> Source: https://wiki.resonite.com/Component:GlueTool

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/7/70/GlueToolComponent.png/510px-GlueToolComponent.png)](https://wiki.resonite.com/File:GlueToolComponent.png) **Glue Tool** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

See [Glue Tool](https://wiki.resonite.com/Glue_Tool "Glue Tool").

> Warning, this tool doesn't know the difference between art and flesh.
>
> —Creator Jam

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
| `GlueMode` | **[Glue.Mode](https://wiki.resonite.com/Component:Glue#Mode "Component:Glue")** | The mode that newly created [Glue](https://wiki.resonite.com/Component:Glue "Component:Glue") spheres should be set to. |
| `_indicatorColor` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The field to drive with the current indicator color. |
| `_activeGlues` | _[list](https://wiki.resonite.com/Type:SyncRefList%601 "Type:SyncRefList`1")_ of **[Glue](https://wiki.resonite.com/Component:Glue "Component:Glue")** | List of glue AOE fields to glue when hitting secondary. |

Fields
Collapse

## See Also

- [Component:Glue](https://wiki.resonite.com/Component:Glue "Component:Glue")
- [Glue Tool](https://wiki.resonite.com/Glue_Tool "Glue Tool")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:GlueTool&oldid=98019](https://wiki.resonite.com/index.php?title=Component:GlueTool&oldid=98019)"

Contents