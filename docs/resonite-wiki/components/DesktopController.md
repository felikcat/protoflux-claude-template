# Component:DesktopController

> Source: https://wiki.resonite.com/Component:DesktopController

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/a/aa/DesktopControllerComponent.png/510px-DesktopControllerComponent.png)](https://wiki.resonite.com/File:DesktopControllerComponent.png) **Desktop Controller** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **DesktopController** component is used to control the desktop through the game dash.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `FollowCursor` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | whether the desktop cursor should follow the Resonite dash cursor when not clicking. |
| `LegacyInputMode` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to use the legacy input system for desktop interaction. |
| `Brightness` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | how bright the desktop display should be in the dash. |
| `Opacity` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | how transparent the desktop display should be in the dash. |
| `_displayColor` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color of the display texture to drive |
| `_displayRect` | **[RectTransform](https://wiki.resonite.com/Component:RectTransform "Component:RectTransform")** | The UIX size rectangle for the display texture. |
| `_desktopTexture` | **[DesktopTextureProvider](https://wiki.resonite.com/Component:DesktopTextureProvider "Component:DesktopTextureProvider")** | The texture displaying the desktop. |
| `_interactionRelay` | **[DesktopInteractionRelay](https://wiki.resonite.com/Component:DesktopInteractionRelay "Component:DesktopInteractionRelay")** | The relay allowing for system Desktop interaction. |
| `_currentControl` | **[DesktopControlDialog](https://wiki.resonite.com/Component:DesktopControlDialog "Component:DesktopControlDialog")** | The current dialogue being used to change settings for this component. |

Fields
Collapse

## Examples

Used in the desktop dash tab to control and view the desktop.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:DesktopController&oldid=94515](https://wiki.resonite.com/index.php?title=Component:DesktopController&oldid=94515)"

Contents