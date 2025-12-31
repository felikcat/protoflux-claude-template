# Component:Button

> Source: https://wiki.resonite.com/Component:Button

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:Button&diff=95802) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/f/f0/ButtonComponent.png/510px-ButtonComponent.png)](https://wiki.resonite.com/File:ButtonComponent.png) **Button** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Button** component is an interactive [UIX](https://wiki.resonite.com/UIX "UIX") element that allows for users to click on its [RectTransform](https://wiki.resonite.com/Component:RectTransform "Component:RectTransform"). It can provide visual feedback by altering the colors of graphics on the RectTransform [Slot](https://wiki.resonite.com/Slot "Slot"), such as the [Image](https://wiki.resonite.com/Component:Image "Component:Image") component. This is able to trigger several other components, such as [Text Field](https://wiki.resonite.com/Component:TextField "Component:TextField"), by using the [Button Events](https://wiki.resonite.com/Button_Events "Button Events") system.

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `BaseColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color that all other tints will be based on |
| `ColorDrivers` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[ColorDriver](https://wiki.resonite.com/index.php?title=Type:ColorDriver&action=edit&redlink=1 "Type:ColorDriver (page does not exist)")** | A list of sets of colors. Each one points at another component's color, and determines how it looks normally, when highlighted, when pressed, and when disabled |
| `__legacy_NormalColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | Legacy normal button color. |
| `__legacy_HighlightColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | Legacy highlight button color. |
| `__legacy_PressColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | Legacy press button color. |
| `__legacy_DisabledColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | Legacy disabled button color. |
| `__legacy_TintColorMode` | **[ColorMode](https://wiki.resonite.com/index.php?title=Type:ColorMode&action=edit&redlink=1 "Type:ColorMode (page does not exist)")** | Legacy tint button color. |
| `__legacy_ColorDrive` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | Legacy color drive button. |
| `IsPressed` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | True if the button is being pressed |
| `IsHovering` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | True if someone is hovering over the button |
| `HoverVibrate` | **[VibratePreset](https://wiki.resonite.com/Type:VibratePreset "Type:VibratePreset")** | How a controller should vibrate when hovering over this button |
| `PressVibrate` | **[VibratePreset](https://wiki.resonite.com/Type:VibratePreset "Type:VibratePreset")** | How a controller should vibrate when pressing this button |
| `ClearFocusOnPress` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | If set, will defocus any currently focused [TextEditor](https://wiki.resonite.com/Component:TextEditor "Component:TextEditor"), [DesktopInteractionRelay](https://wiki.resonite.com/index.php?title=DesktopInteractionRelay&action=edit&redlink=1 "DesktopInteractionRelay (page does not exist)"), or any other [IFocusable](https://wiki.resonite.com/index.php?title=IFocusable&action=edit&redlink=1 "IFocusable (page does not exist)") when this button is pressed. Defaults to true. |
| `PassThroughHorizontalMovement` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether or not press-and-drag movement should be passed to higher components<br>(such as [Scroll Rects](https://wiki.resonite.com/index.php?title=Scroll_Rect_(Component)&action=edit&redlink=1 "Scroll Rect (Component) (page does not exist)")) |
| `PassThroughVerticalMovement` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether or not press-and-drag movement should be passed to higher components<br>(such as [Scroll Rects](https://wiki.resonite.com/index.php?title=Scroll_Rect_(Component)&action=edit&redlink=1 "Scroll Rect (Component) (page does not exist)")) |
| `RequireLockInToPress` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Internal. Defaults to false. |
| `RequireInitialPress` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Internal - Check for the initial press of the button. Defaults to true. |
| `PressPoint` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The (x,y) coordinate where the button is being pressed |
| `SendSlotEvents` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | If set, all Pressing, Pressed, Released, HoverEnter, HoverStay, and HoverLeave events are sent to all [IButtonPressReceiver](https://wiki.resonite.com/index.php?title=IButtonPressReceiver&action=edit&redlink=1 "IButtonPressReceiver (page does not exist)") components within this component's slot. Defaults to true. |
| `Pressed` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | Delegate. If set, this function is called with the Pressed event. Defaults to unset. |
| `Pressing` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | Delegate. If set, this function is called with the Pressing event. Defaults to unset. |
| `Released` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | Delegate. If set, this function is called with the Released event. Defaults to unset. |
| `HoverEnter` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | Delegate. If set, this function is called with the HoverEnter event. Defaults to unset. |
| `HoverStay` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | Delegate. If set, this function is called with the HoverStay event. Defaults to unset. |
| `HoverLeave` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | Delegate. If set, this function is called with the HoverLeave event. Defaults to unset. |

Fields
Collapse

## Usage

This can be used with [ProtoFlux](https://wiki.resonite.com/ProtoFlux "ProtoFlux"), and specifically the [Button Events](https://wiki.resonite.com/ProtoFlux:Button_Events "ProtoFlux:Button Events") node. Allowing it to fire [Impulses](https://wiki.resonite.com/Impulses "Impulses") from this [IButton](https://wiki.resonite.com/Type:IButton "Type:IButton") reference.

## Examples

[![A button from the Resonite Essentials folder.](https://wiki.resonite.com/images/thumb/9/9a/UIX_Button_Example_01.png/300px-UIX_Button_Example_01.png)](https://wiki.resonite.com/File:UIX_Button_Example_01.png) A button from the Resonite Essentials folder.

There is a button UI Preset from the [Resonite Essentials](https://wiki.resonite.com/Resonite_Essentials "Resonite Essentials") folder that users can use as a starting point for buttons.

Here is [ProbablePrime](https://wiki.resonite.com/User:ProbablePrime "User:ProbablePrime")'s tutorial on Buttons:

![](https://i.ytimg.com/vi/lCGfFJYOj3o/hqdefault.jpg)

[OLD: Neos VR Tutorial: UIX Pt.2 Materials, Buttons and Text](https://www.youtube-nocookie.com/embed/lCGfFJYOj3o?autoplay=1)

Load video

YouTube

YouTube might collect personal data. [Privacy Policy](https://www.youtube.com/howyoutubeworks/user-settings/privacy/)

ContinueDismiss

## Related Components

## See Also

- [Component:TouchButton](https://wiki.resonite.com/Component:TouchButton "Component:TouchButton")
- [Component:LegacyButton](https://wiki.resonite.com/Component:LegacyButton "Component:LegacyButton")
- [Component:ButtonRelay](https://wiki.resonite.com/Component:ButtonRelay "Component:ButtonRelay")
- [Component:ButtonToggle](https://wiki.resonite.com/Component:ButtonToggle "Component:ButtonToggle")
- [Component:PhysicalButton](https://wiki.resonite.com/Component:PhysicalButton "Component:PhysicalButton")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:Button&oldid=95802](https://wiki.resonite.com/index.php?title=Component:Button&oldid=95802)"

Contents