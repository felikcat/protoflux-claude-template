# Component:GaussianSplatTool

> Source: https://wiki.resonite.com/Component:GaussianSplatTool

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/0/0f/GaussianSplatToolComponent.png/510px-GaussianSplatToolComponent.png)](https://wiki.resonite.com/File:GaussianSplatToolComponent.png) **Gaussian Splat Tool** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **GaussianSplatTool** component can be applied to a [slot](https://wiki.resonite.com/Slot "Slot") to create a [Gaussian Splat Tool](https://wiki.resonite.com/Gaussian_Splat_Tool "Gaussian Splat Tool"), used to manipulate a [Gaussian Splat](https://wiki.resonite.com/Gaussian_Splat "Gaussian Splat") in [3D space](https://wiki.resonite.com/Slot_transforms#Coordinate_spaces "Slot transforms").

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
| `Mode` | **[GaussianSplatTool+OperationMode](https://wiki.resonite.com/index.php?title=Type:GaussianSplatTool%2BOperationMode&action=edit&redlink=1 "Type:GaussianSplatTool+OperationMode (page does not exist)")** | The selected mode for this Gaussian Splat Tool. |
| `BoxSelectionTemplate` | **[GaussianSplatTool+BoxInterface](https://wiki.resonite.com/index.php?title=Type:GaussianSplatTool%2BBoxInterface&action=edit&redlink=1 "Type:GaussianSplatTool+BoxInterface (page does not exist)")** | The templete used to show the user what is being cropped when using the box. |
| `SphereSelectionTemplate` | **[GaussianSplatTool+SphereInterface](https://wiki.resonite.com/index.php?title=Type:GaussianSplatTool%2BSphereInterface&action=edit&redlink=1 "Type:GaussianSplatTool+SphereInterface (page does not exist)")** | The templete used to show the user what is being cropped when using the sphere. |
| `CylinderSelectionTemplate` | **[GaussianSplatTool+CylinderInterface](https://wiki.resonite.com/index.php?title=Type:GaussianSplatTool%2BCylinderInterface&action=edit&redlink=1 "Type:GaussianSplatTool+CylinderInterface (page does not exist)")** | The templete used to show the user what is being cropped when using the cylinder. |
| `_activeBox` | **[GaussianSplatTool+BoxInterface](https://wiki.resonite.com/index.php?title=Type:GaussianSplatTool%2BBoxInterface&action=edit&redlink=1 "Type:GaussianSplatTool+BoxInterface (page does not exist)")** | Internal - References the active box. |
| `_activeSphere` | **[GaussianSplatTool+SphereInterface](https://wiki.resonite.com/index.php?title=Type:GaussianSplatTool%2BSphereInterface&action=edit&redlink=1 "Type:GaussianSplatTool+SphereInterface (page does not exist)")** | Internal - References the active sphere. |
| `_activeCylinder` | **[GaussianSplatTool+CylinderInterface](https://wiki.resonite.com/index.php?title=Type:GaussianSplatTool%2BCylinderInterface&action=edit&redlink=1 "Type:GaussianSplatTool+CylinderInterface (page does not exist)")** | Internal - References the active cylinder. |

Fields
Collapse

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:GaussianSplatTool&oldid=113587](https://wiki.resonite.com/index.php?title=Component:GaussianSplatTool&oldid=113587)"

Contents