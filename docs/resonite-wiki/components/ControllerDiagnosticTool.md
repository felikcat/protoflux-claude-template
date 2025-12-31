# Component:ControllerDiagnosticTool

> Source: https://wiki.resonite.com/Component:ControllerDiagnosticTool

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/5/57/ControllerDiagnosticToolComponent.png/510px-ControllerDiagnosticToolComponent.png)](https://wiki.resonite.com/File:ControllerDiagnosticToolComponent.png) **Controller Diagnostic Tool** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ControllerDiagnosticTool** component is a tool that gives information on controller info for the hand its equipped on. For more info see [Controller Diagnostic Tool](https://wiki.resonite.com/Controller_Diagnostic_Tool "Controller Diagnostic Tool").

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
| `_text` | **[TextRenderer](https://wiki.resonite.com/Component:TextRenderer "Component:TextRenderer")** | The text renderer to fill with controller diagnostic info to display. |

Fields
Collapse

## See Also

- [Controller Diagnostic Tool](https://wiki.resonite.com/Controller_Diagnostic_Tool "Controller Diagnostic Tool")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ControllerDiagnosticTool&oldid=95675](https://wiki.resonite.com/index.php?title=Component:ControllerDiagnosticTool&oldid=95675)"

Contents