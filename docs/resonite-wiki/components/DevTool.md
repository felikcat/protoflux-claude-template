# Component:DevTool

> Source: https://wiki.resonite.com/Component:DevTool

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/d/d4/DevToolComponent.png/510px-DevToolComponent.png)](https://wiki.resonite.com/File:DevToolComponent.png) **Dev Tool** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

Detailed information can be located at [Dev Tool](https://wiki.resonite.com/Dev_Tool "Dev Tool").

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
| `SelectionMode` | **[DevTool.Selection](https://wiki.resonite.com/Component:DevTool#Selection)** | See [Selection section](https://wiki.resonite.com/Component:DevTool#Selection). |
| `InteractionMode` | **[DevTool.Interaction](https://wiki.resonite.com/Component:DevTool#Interaction)** | See [Interaction section](https://wiki.resonite.com/Component:DevTool#Interaction). |
| `_selectedAnchor` | **[PointAnchor](https://wiki.resonite.com/Component:PointAnchor "Component:PointAnchor")** | The point anchor which is part of a gizmo this tool is moving currently. |
| `_selectedAnchorHighlight` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot being used to indicate what gizmo is currently being moved. Is an icosphere. |
| `_material` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[OverlayFresnelMaterial](https://wiki.resonite.com/OverlayFresnelMaterial "OverlayFresnelMaterial")** | The visual material used for the default cone mesh. |
| `_currentGizmo` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The gizmo that the dev tool is currently targeting for gizmo options. |
| `_previousGizmo` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The previous gizmo that the dev tool targeted for gizmo options. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `ToggleDevMode:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | See [Dev Tool](https://wiki.resonite.com/Dev_Tool "Dev Tool"). |
| `DeselectAll:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | See [Dev Tool](https://wiki.resonite.com/Dev_Tool "Dev Tool"). |
| `OpenCreate:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | See [Dev Tool](https://wiki.resonite.com/Dev_Tool "Dev Tool"). |
| `OpenInspector:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | See [Dev Tool](https://wiki.resonite.com/Dev_Tool "Dev Tool"). |
| `OpenGizmoOptions:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | See [Dev Tool](https://wiki.resonite.com/Dev_Tool "Dev Tool"). |
| `SelectParent:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | See [Dev Tool](https://wiki.resonite.com/Dev_Tool "Dev Tool"). |
| `ToggleSpace:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | See [Dev Tool](https://wiki.resonite.com/Dev_Tool "Dev Tool"). |
| `SetTranslation:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | See [Dev Tool](https://wiki.resonite.com/Dev_Tool "Dev Tool"). |
| `SetRotation:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | See [Dev Tool](https://wiki.resonite.com/Dev_Tool "Dev Tool"). |
| `SetScale:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | See [Dev Tool](https://wiki.resonite.com/Dev_Tool "Dev Tool"). |
| `OnOpenParent:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | See [Dev Tool](https://wiki.resonite.com/Dev_Tool "Dev Tool"). |
| `SetTranslation:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | See [Dev Tool](https://wiki.resonite.com/Dev_Tool "Dev Tool"). |
| `SetRotation:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | See [Dev Tool](https://wiki.resonite.com/Dev_Tool "Dev Tool"). |
| `SetScale:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | See [Dev Tool](https://wiki.resonite.com/Dev_Tool "Dev Tool"). |
| ``ActivateGizmo:ButtonEventHandler`1<Component>`` | **[ButtonEventHandler\`1](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler%601&action=edit&redlink=1 "Type:ButtonEventHandler`1 (page does not exist)") < [Component](https://wiki.resonite.com/Type:Component "Type:Component") >** | ✓ | See [Dev Tool](https://wiki.resonite.com/Dev_Tool "Dev Tool"). |
| `DestroySelected:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | See [Dev Tool](https://wiki.resonite.com/Dev_Tool "Dev Tool"). |
| `DestroyConfirm:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | See [Dev Tool](https://wiki.resonite.com/Dev_Tool "Dev Tool"). |
| `OnCancelMenu:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | See [Dev Tool](https://wiki.resonite.com/Dev_Tool "Dev Tool"). |
| `OnGizmoReplaced:SlotGizmo.SlotGizmoReplacement` | **[SlotGizmo.SlotGizmoReplacement](https://wiki.resonite.com/Component:SlotGizmo#SlotGizmoReplacement "Component:SlotGizmo")** | ✓ | See [Dev Tool](https://wiki.resonite.com/Dev_Tool "Dev Tool"). |

Triggers
Collapse

## Selection

- **Selection**: Sets the selection mode for the tool (select by using the secondary action):

  - _Single_: Select single object. Selecting an unselected object deselects any other selected object. Selecting a selected object unselects that object.
  - _Multi_: Select multiple objects. Selecting an unselected object adds that object to the selected objects. Selecting a selected object unselects that object.

## Interaction

- **Interaction**: What gizmo transformation should be relative to:

  - _Tip_: Gizmo transformation is relative to the tool's tip.
  - _Projection_: Gizmo transformation is relative to the projected point.

## Examples

The DevTool component can be used on it's own to create a [Developer Tool](https://wiki.resonite.com/Dev_Tool "Dev Tool") or be used in a [ToolMultiplexer](https://wiki.resonite.com/Component:ToolMultiplexer "Component:ToolMultiplexer") to create a MultiTool.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:DevTool&oldid=98421](https://wiki.resonite.com/index.php?title=Component:DevTool&oldid=98421)"

Contents