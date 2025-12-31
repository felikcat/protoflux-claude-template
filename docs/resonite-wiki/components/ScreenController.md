# Component:ScreenController

> Source: https://wiki.resonite.com/Component:ScreenController

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/1/19/ScreenControllerComponent.png/510px-ScreenControllerComponent.png)](https://wiki.resonite.com/File:ScreenControllerComponent.png) **Screen Controller** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ScreenController** component is used mainly in desktop and is found on user roots. It is used to control the screen controls like third person in the game.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `TransitionSpeed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How fast to transition the camera between different modes. |
| `PointerController` | **[PointerInteractionController](https://wiki.resonite.com/Component:PointerInteractionController "Component:PointerInteractionController")** | The pointer component handling inspector interactions. |
| `ActiveTargetting` | **[IViewTargettingController](https://wiki.resonite.com/index.php?title=Type:IViewTargettingController&action=edit&redlink=1 "Type:IViewTargettingController (page does not exist)")** | The view controller targeting mechanism for stuff like UIX targeting. |
| `Head` | **[HeadSimulator](https://wiki.resonite.com/Component:HeadSimulator "Component:HeadSimulator")** | The component handling head control. |
| `LeftHand` | **[HandSimulator](https://wiki.resonite.com/Component:HandSimulator "Component:HandSimulator")** | The component handing the left hand control. |
| `RightHand` | **[HandSimulator](https://wiki.resonite.com/Component:HandSimulator "Component:HandSimulator")** | The component handling the right hand control. |
| `_previousTargetting` | **[IViewTargettingController](https://wiki.resonite.com/index.php?title=Type:IViewTargettingController&action=edit&redlink=1 "Type:IViewTargettingController (page does not exist)")** | The previously used targeting controller. |
| `_firstPerson` | **[FirstPersonTargettingController](https://wiki.resonite.com/Component:FirstPersonTargettingController "Component:FirstPersonTargettingController")** | The component to handle first person object targeting. |
| `_thirdPerson` | **[ThirdPersonTargettingController](https://wiki.resonite.com/Component:ThirdPersonTargettingController "Component:ThirdPersonTargettingController")** | The component to handle third person object targeting. |
| `_uiCamera` | **[UI\_TargettingController](https://wiki.resonite.com/Component:UI_TargettingController "Component:UI TargettingController")** | The targetting controller used for UIX targeting. |
| `_freeformCamera` | **[FreeformTargettingController](https://wiki.resonite.com/Component:FreeformTargettingController "Component:FreeformTargettingController")** | The targetting controller used for third person targetting like freeform camera mode in desktop. |

Fields
Collapse

## Usage

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ScreenController&oldid=106553](https://wiki.resonite.com/index.php?title=Component:ScreenController&oldid=106553)"

Contents