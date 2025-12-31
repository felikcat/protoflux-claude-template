# Component:InteractiveCameraUserItem

> Source: https://wiki.resonite.com/Component:InteractiveCameraUserItem

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/0/0c/InteractiveCameraUserItemComponent.png/510px-InteractiveCameraUserItemComponent.png)](https://wiki.resonite.com/File:InteractiveCameraUserItemComponent.png) **Interactive Camera User Item** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

See [Camera](https://wiki.resonite.com/Camera "Camera").

Used to handle the items for each user for the interactive camera settings.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Control` | **[InteractiveCameraControl](https://wiki.resonite.com/Component:InteractiveCameraControl "Component:InteractiveCameraControl")** | The root camera control settings panel. |
| `_username` | **[Text](https://wiki.resonite.com/Component:Text "Component:Text")** | The username of the user this item refers to. |
| `_voiceDefault` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | Capture this user's voice as their default voice setting. |
| `_voiceMute` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | Capture this user's voice as the mute voice setting. |
| `_voiceShout` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | Capture this user's voice as the shout voice setting. |
| `_voiceBroadcast` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | Capture this user's voice as the broadcast voice setting. |
| `_groupAuto` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | Set this user's group inclusion and exclusion modes to default. |
| `_groupExclude` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | Set this user's group inclusion to never. |
| `_groupInclude` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | Set this user's group inclusion to always. |
| `_cameraOperator` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | Make this user able to interact with the camera. |
| `_framingTarget` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | Make this user a framing target when framing the scene. |
| `_volumeSlider` | **[Slider\`1](https://wiki.resonite.com/Component:Slider%601 "Component:Slider`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | The user's voice volume when capturing their voice. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `OnVoiceDefault:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | A setting changing handler for the panel. |
| `OnVoiceMute:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | A setting changing handler for the panel. |
| `OnVoiceShout:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | A setting changing handler for the panel. |
| `OnVoiceBroadcast:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | A setting changing handler for the panel. |
| `OnGroupExclude:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | A setting changing handler for the panel. |
| `OnGroupAuto:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | A setting changing handler for the panel. |
| `OnGroupInclude:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | A setting changing handler for the panel. |
| `OnToggleOperator:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | A setting changing handler for the panel. |
| `OnSetFramingTarget:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | A setting changing handler for the panel. |

Triggers
Collapse

## Usage

See [Camera](https://wiki.resonite.com/Camera "Camera").

## Examples

See [Camera](https://wiki.resonite.com/Camera "Camera").

## See Also

- [Camera](https://wiki.resonite.com/Camera "Camera")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:InteractiveCameraUserItem&oldid=98933](https://wiki.resonite.com/index.php?title=Component:InteractiveCameraUserItem&oldid=98933)"

Contents