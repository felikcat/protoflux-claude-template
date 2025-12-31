# Component:MeshVisibilityToggleTool

> Source: https://wiki.resonite.com/Component:MeshVisibilityToggleTool

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/a/a6/MeshVisibilityToggleToolComponent.png/510px-MeshVisibilityToggleToolComponent.png)](https://wiki.resonite.com/File:MeshVisibilityToggleToolComponent.png) **Mesh Visibility Toggle Tool** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

See [Mesh Visibility Tool](https://wiki.resonite.com/Mesh_Visibility_Tool "Mesh Visibility Tool").

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
| `ApplyToObjectRoot` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to search for an object root in order to apply to all meshes under that root. |
| `SetShadowCastMode` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [ShadowCastMode](https://wiki.resonite.com/Type:ShadowCastMode "Type:ShadowCastMode") >** | Whether to set the meshes shadow mode and what to set it to. |

Fields
Collapse

## Usage

See [Mesh Visibility Tool](https://wiki.resonite.com/Mesh_Visibility_Tool "Mesh Visibility Tool").

## Examples

See [Mesh Visibility Tool](https://wiki.resonite.com/Mesh_Visibility_Tool "Mesh Visibility Tool").

## See Also

- [Mesh Visibility Tool](https://wiki.resonite.com/Mesh_Visibility_Tool "Mesh Visibility Tool")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:MeshVisibilityToggleTool&oldid=94943](https://wiki.resonite.com/index.php?title=Component:MeshVisibilityToggleTool&oldid=94943)"

Contents