# Component:ShapeTool

> Source: https://wiki.resonite.com/Component:ShapeTool

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/e/e3/ShapeToolComponent.png/510px-ShapeToolComponent.png)](https://wiki.resonite.com/File:ShapeToolComponent.png) **Shape Tool** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

See [Shape Tool](https://wiki.resonite.com/Shape_Tool "Shape Tool").

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
| `activeShape` | **[ShapeTool.Shape](https://wiki.resonite.com/Component:ShapeTool#Shape)** | The shape to draw. |
| `shapes` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[SyncRef\`1](https://wiki.resonite.com/Type:SyncRef%601 "Type:SyncRef`1") < [Slot](https://wiki.resonite.com/Type:Slot "Type:Slot") >** | A list of shapes to switch between depending on `activeShape` for the tool tips visual. |
| `Material` | **[Material](https://wiki.resonite.com/Type:Material "Type:Material")** | The material to use when drawing shapes. |

Fields
Collapse

## Shape

| Name | Value | Description |
| --- | --- | --- |
| `Cube` | 0 | Draw a cube. |
| `Sphere` | 1 | Draw a smooth sphere. |
| `Cylinder` | 2 | Draw a cylinder. |
| `Cone` | 3 | Draw a cone. |
| `Quad` | 4 | Draw a 2d square. |
| `FlatSphere` | 5 | Draw a flat shaded icosphere. |

Values

## See Also

- [Shape Tool](https://wiki.resonite.com/Shape_Tool "Shape Tool")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ShapeTool&oldid=97735](https://wiki.resonite.com/index.php?title=Component:ShapeTool&oldid=97735)"

Contents