# Component:TouchButton

> Source: https://wiki.resonite.com/Component:TouchButton

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:TouchButton&diff=94816) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/5/54/TouchButtonComponent.png/510px-TouchButtonComponent.png)](https://wiki.resonite.com/File:TouchButtonComponent.png) **Touch Button** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **TouchButton** component is used to make a physical button with no press depth that is instantly pressable upon click or touch. For a button with press depth, please see [PhysicalButton](https://wiki.resonite.com/Component:PhysicalButton "Component:PhysicalButton").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `IsPressed` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the button is pressed or not |
| `IsHovering` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the button is being pointed at with the laser in the case of a touch button |
| `AcceptPhysicalTouch` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to allow [Component:TipTouchSources](https://wiki.resonite.com/Component:TipTouchSource "Component:TipTouchSource") to interact with/activate this component. |
| `AcceptRemoteTouch` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this component allows interaction via the user's interaction laser. |
| `AcceptOutOfSightTouch` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether or not to allow interaction with this component if it is out of the user's view. |
| `EditModeOnly` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this button will only work if the user is in [Edit Mode](https://wiki.resonite.com/Edit_Mode "Edit Mode") |
| `ActiveUserFilter` | **[ActiveUserHandling](https://wiki.resonite.com/Type:ActiveUserHandling "Type:ActiveUserHandling")** | How to handle user interaction depending on active user. |
| `Pressed` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | The [Sync Delegate](https://wiki.resonite.com/Sync_Delegate "Sync Delegate") to call when the button is pressed. |
| `Pressing` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | The [Sync Delegate](https://wiki.resonite.com/Sync_Delegate "Sync Delegate") to call when the button is being pressed every game tick. |
| `Released` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | The [Sync Delegate](https://wiki.resonite.com/Sync_Delegate "Sync Delegate") to call when the button is released. |
| `BeginPressVibration` | **[VibratePreset](https://wiki.resonite.com/Type:VibratePreset "Type:VibratePreset")** | What vibration to send when this button is starting to be pressed. |
| `PressVibration` | **[VibratePreset](https://wiki.resonite.com/Type:VibratePreset "Type:VibratePreset")** | What vibration to send when this button is pressed. |
| `HoverVibration` | **[VibratePreset](https://wiki.resonite.com/Type:VibratePreset "Type:VibratePreset")** | What vibration to send when this button is hovered over via laser. |
| `Label` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | The field that represents this button's label. |

Fields
Collapse

## Usage

Used in boopers and buttons where [PhysicalButton](https://wiki.resonite.com/Component:PhysicalButton "Component:PhysicalButton") is a bad choice because the button press needs to have no press depth. In the case where the user does want press depth, use [PhysicalButton](https://wiki.resonite.com/Component:PhysicalButton "Component:PhysicalButton").

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [IButton](https://wiki.resonite.com/Type:IButton "Type:IButton") For a list of button types.

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:TouchButton&oldid=94816](https://wiki.resonite.com/index.php?title=Component:TouchButton&oldid=94816)"

Contents