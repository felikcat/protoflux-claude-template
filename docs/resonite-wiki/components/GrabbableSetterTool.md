# Component:GrabbableSetterTool

> Source: https://wiki.resonite.com/Component:GrabbableSetterTool

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/6/66/GrabbableSetterToolComponent.png/510px-GrabbableSetterToolComponent.png)](https://wiki.resonite.com/File:GrabbableSetterToolComponent.png) **Grabbable Setter Tool** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

See [Grabbable Setter Tool](https://wiki.resonite.com/Grabbable_Setter_Tool "Grabbable Setter Tool").

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
| `ApplyToObjectRoot` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to search for a root when hitting a collider before applying the grabbable to that slot. |
| `SetScalable` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the applied grababble should be scalable. |
| `_indicatorColor` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color to change for indicating this tool's settings. Used for the default cone model usually. |

Fields
Collapse

## See Also

- [Grabbable Setter Tool](https://wiki.resonite.com/Grabbable_Setter_Tool "Grabbable Setter Tool")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:GrabbableSetterTool&oldid=94785](https://wiki.resonite.com/index.php?title=Component:GrabbableSetterTool&oldid=94785)"

Contents