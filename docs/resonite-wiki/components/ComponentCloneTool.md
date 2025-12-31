# Component:ComponentCloneTool

> Source: https://wiki.resonite.com/Component:ComponentCloneTool

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/9/9e/ComponentCloneToolComponent.png/510px-ComponentCloneToolComponent.png)](https://wiki.resonite.com/File:ComponentCloneToolComponent.png) **Component Clone Tool** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

See [Component Clone Tool](https://wiki.resonite.com/Component_Clone_Tool "Component Clone Tool")

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
| `ApplyToObjectRoot` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to search for an object root to put the Component onto rather than the hit component or slot. |
| `EnsureSingleInstance` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the tool should delete existing components of the same type before adding the ones from the template. |
| `AllowPickup` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the tool can add components to its template list with secondary. |
| `_label` | **[TextRenderer](https://wiki.resonite.com/Component:TextRenderer "Component:TextRenderer")** | The label giving information on this tool. |
| `_templateRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot this tool is using to store its list of components to place onto other slots. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `OnClearTemplate:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Handles clearing the components on `_templateRoot` |

Triggers
Collapse

## Usage

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ComponentCloneTool&oldid=98351](https://wiki.resonite.com/index.php?title=Component:ComponentCloneTool&oldid=98351)"

Contents