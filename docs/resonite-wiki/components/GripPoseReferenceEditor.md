# Component:GripPoseReferenceEditor

> Source: https://wiki.resonite.com/Component:GripPoseReferenceEditor

Collapse **Component image**

[File:GripPoseReferenceEditorComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=GripPoseReferenceEditorComponent.png "File:GripPoseReferenceEditorComponent.png") **Grip Pose Reference Editor** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **GripPoseReferenceEditor** component handles the [UI Edit Mode](https://wiki.resonite.com/UI_Edit_Mode "UI Edit Mode") behavior of adjusting [Raw Data Tools](https://wiki.resonite.com/Component:RawDataTool "Component:RawDataTool") in the user's hand. See [UI Edit Mode](https://wiki.resonite.com/UI_Edit_Mode "UI Edit Mode") for more information.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `ReferenceRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The root slot of the tool tip holder. |
| `Item` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The root slot of the tooltip being adjusted. |
| `Slider` | **[Slider](https://wiki.resonite.com/Component:Slider "Component:Slider")** | The slider to use to adjust the tool tip during grabbing. |
| `PoseReference` | **[GripPoseReference](https://wiki.resonite.com/Component:GripPoseReference "Component:GripPoseReference")** | The grip pose reference to be modifying. |
| `HideVisualOnEnd` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Hide the visual when it's not being grabbed. |
| `RootPosition` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The root position of the gripping pose reference. |
| `RootRotation` | **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The root rotation of the gripping pose reference. |
| `RootScale` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The root scale of the gripping pose reference. |

Fields
Collapse

## Usage

Not used directly by the user. Please see [UI Edit Mode](https://wiki.resonite.com/UI_Edit_Mode "UI Edit Mode").

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:GripPoseReferenceEditor&oldid=96763](https://wiki.resonite.com/index.php?title=Component:GripPoseReferenceEditor&oldid=96763)"

Contents