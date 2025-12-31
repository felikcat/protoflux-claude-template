# Component:GripPoseReference

> Source: https://wiki.resonite.com/Component:GripPoseReference

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/b/be/GripPoseReferenceComponent.png/510px-GripPoseReferenceComponent.png)](https://wiki.resonite.com/File:GripPoseReferenceComponent.png) **Grip Pose Reference** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **GripPoseReference** component is placed under [Tools](https://wiki.resonite.com/Tools "Tools") to tell them how they should be positioned when equipped.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `HandSide` | **[Chirality](https://wiki.resonite.com/Type:Chirality "Type:Chirality")** | The hand side this grip pose should |
| `_rootPos` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The root position of the tooltip. |
| `TipReference` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | the slot for the tool tips tip in question. |
| `ShowVisual` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to show the adjustment visual. |
| `DisableSlider` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to disable adjusting this grip pose. |
| `_activeVisual` | _direct_ **[CleanupRef\`1](https://wiki.resonite.com/Type:CleanupRef%601 "Type:CleanupRef`1") < [Slot](https://wiki.resonite.com/Type:Slot "Type:Slot") >** | The current adjustment visual. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `GrabCheck:GrabCheck` | **[GrabCheck](https://wiki.resonite.com/Type:GrabCheck "Type:GrabCheck")** | ✓ | The grab check to see if the hand grabbing can grab the grabbable assigned with this. This grab check is the only grab check in the game that can exclude a hand. This is useful for making an item only grabbable with the right or left hand. This is not static, and needs the component. The hand specified in the component is the one "whitelisted" in the grab check. |

Triggers
Collapse

## Usage

To create a simple object using GripPoseReference, add the RawDataTool slot to the root of the object containing the mesh. This will automatically add the GripPoseReference slots. To edit the pose, enter [UI Edit Mode](https://wiki.resonite.com/UI_Edit_Mode "UI Edit Mode") with the Left or Right GripPoseReference slot selected in Scene Inspector then adjust the object pose in one hand's grip with your off hand.

When the TipReference field is set, equipping the tool will align your tip reference (usually at the tip of your index finger) to the provided slot and ignore the transform of the grip pose. It is recommended to use this for custom tools which are supposed to have similar positioning to most of the default tools such as the [Dev Tool](https://wiki.resonite.com/Dev_Tool "Dev Tool").

## Interaction with hand poser

When grabbing or equipping a tool which defines a GripPoseReference without a set TipReference, the initial location from which the grip pose is applied is interpolated based on the location of the fingers and the HandRoot configured in the corresponding [HandPoser](https://wiki.resonite.com/Component:HandPoser "Component:HandPoser").

For avatars with commonly-shaped hands with at least three fingers, this interpolated pose is usually close enough that, if you position the GripPoseReference correctly for one avatar, it should also be positioned decently well for most other avatars.

## See Also

- [Tools](https://wiki.resonite.com/Tools "Tools")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:GripPoseReference&oldid=111593](https://wiki.resonite.com/index.php?title=Component:GripPoseReference&oldid=111593)"

Contents