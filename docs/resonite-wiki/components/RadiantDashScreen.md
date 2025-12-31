# Component:RadiantDashScreen

> Source: https://wiki.resonite.com/Component:RadiantDashScreen

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/9/9a/RadiantDashScreenComponent.png/510px-RadiantDashScreenComponent.png)](https://wiki.resonite.com/File:RadiantDashScreenComponent.png) **Radiant Dash Screen** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

See [Dash menu](https://wiki.resonite.com/Dash_menu "Dash menu").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Icon` | **[Uri](https://wiki.resonite.com/Type:Uri "Type:Uri")** | The icon for this screen. |
| `ActiveColor` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX") >** | The color when this screen is active. |
| `Label` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The name of this screen. |
| `ScreenEnabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this screen is enabled. |
| `BaseResolution` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The resolution of this screen. |
| `_screenRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The root of the elements on this screen. |
| `_screenCanvas` | **[Canvas](https://wiki.resonite.com/Component:Canvas "Component:Canvas")** | The canvas being used to render this screen. |
| `_modalOverlayManager` | **[ModalOverlayManager](https://wiki.resonite.com/Component:ModalOverlayManager "Component:ModalOverlayManager")** | The manager handling edit mode for this screen. |
| `_button` | **[RadiantDashButton](https://wiki.resonite.com/Component:RadiantDashButton "Component:RadiantDashButton")** | The button to select this screen for the dash. |
| `_iconTexture` | **[Texture2D](https://wiki.resonite.com/Type:Texture2D "Type:Texture2D")** | The texture being used for the icon for this screen. |

Fields
Collapse

## Usage

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:RadiantDashScreen&oldid=106534](https://wiki.resonite.com/index.php?title=Component:RadiantDashScreen&oldid=106534)"

Contents