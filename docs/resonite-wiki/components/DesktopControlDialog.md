# Component:DesktopControlDialog

> Source: https://wiki.resonite.com/Component:DesktopControlDialog

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/b/b6/DesktopControlDialogComponent.png/510px-DesktopControlDialogComponent.png)](https://wiki.resonite.com/File:DesktopControlDialogComponent.png) **Desktop Control Dialog** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **DesktopControlDialog** is used to change the settings for what desktop to control and how to control it.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `InteractionRelay` | **[DesktopInteractionRelay](https://wiki.resonite.com/Component:DesktopInteractionRelay "Component:DesktopInteractionRelay")** | The relay allowing desktop interaction. |
| `Index` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The display to show in a multi monitor settup. |
| `FollowCursor` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | whether the desktop cursor should follow the Resonite dash cursor when not clicking. |
| `Brightness` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | how bright the desktop display should be in the dash. |
| `Opacity` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | how transparent the desktop display should be in the dash. |
| `LegacyInputMode` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to use the legacy input system for desktop interaction. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| ``OnDisplayItemGenerated:Action`2<Display, Slot>`` | **[Action\`2](https://wiki.resonite.com/index.php?title=Type:Action%602&action=edit&redlink=1 "Type:Action`2 (page does not exist)") < [Display](https://wiki.resonite.com/index.php?title=Type:Display&action=edit&redlink=1 "Type:Display (page does not exist)"), [Slot](https://wiki.resonite.com/Type:Slot "Type:Slot") >** | ✓ | Used to handle the creation of new displays and their UI from a [DesktopDisplayLayout](https://wiki.resonite.com/Component:DesktopDisplayLayout "Component:DesktopDisplayLayout"). |
| ``OnSwitchDisplay:ButtonEventHandler`1<Int>`` | **[ButtonEventHandler\`1](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler%601&action=edit&redlink=1 "Type:ButtonEventHandler`1 (page does not exist)") < [Int](https://wiki.resonite.com/Type:Int "Type:Int") >** | ✓ | handles switching the viewed desktop display for this component. |
| `OnOpenKeyboard:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Handles the opening of a keyboard and focusing it to the desktop. |
| `OnOpenStartMenu:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | handles opening a computer's start menu. |

Triggers
Collapse

## Examples

Used in the user dash.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:DesktopControlDialog&oldid=97919](https://wiki.resonite.com/index.php?title=Component:DesktopControlDialog&oldid=97919)"

Contents