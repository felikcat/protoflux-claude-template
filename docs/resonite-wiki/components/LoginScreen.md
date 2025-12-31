# Component:LoginScreen

> Source: https://wiki.resonite.com/Component:LoginScreen

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/5/54/LoginScreenComponent.png/510px-LoginScreenComponent.png)](https://wiki.resonite.com/File:LoginScreenComponent.png) **Login Screen** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **LoginScreen** component is used to handle the dash screen for logging into the game.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Icon` | **[Uri](https://wiki.resonite.com/Type:Uri "Type:Uri")** | The icon of the dash menu tab. |
| `ActiveColor` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX") >** | The color when this dash menu screen tab is selected. |
| `Label` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The text for this dash menu Screen tab. |
| `ScreenEnabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the screen is enabled for viewing. |
| `BaseResolution` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The default resolution of the tab screen. |
| `_screenRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The root slot of the dash menu tab view. |
| `_screenCanvas` | **[Canvas](https://wiki.resonite.com/Component:Canvas "Component:Canvas")** | The canvas being used for the tab view. |
| `_modalOverlayManager` | **[ModalOverlayManager](https://wiki.resonite.com/Component:ModalOverlayManager "Component:ModalOverlayManager")** | The Overlay manager being used for handling edit mode. |
| `_button` | **[RadiantDashButton](https://wiki.resonite.com/Component:RadiantDashButton "Component:RadiantDashButton")** | The button to select this dash menu screen tab. |
| `_iconTexture` | **[Texture2D](https://wiki.resonite.com/Type:Texture2D "Type:Texture2D")** | The texture being used for the icon of this dash menu tab. |

Fields
Collapse

## Usage

Used for logging in.

## Examples

Log in screen. Used internally.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:LoginScreen&oldid=105307](https://wiki.resonite.com/index.php?title=Component:LoginScreen&oldid=105307)"

Contents