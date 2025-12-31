# Component:WorldCloseScreen

> Source: https://wiki.resonite.com/Component:WorldCloseScreen

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/a/a4/WorldCloseScreenComponent.png/510px-WorldCloseScreenComponent.png)](https://wiki.resonite.com/File:WorldCloseScreenComponent.png) **World Close Screen** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **World Close Screen** component is used in the dash and appears when the user asks to close a world. This acts as a conformation. This is also an internally used component.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Icon` | **[Uri](https://wiki.resonite.com/Type:Uri "Type:Uri")** | The icon for this dialogue screen. |
| `ActiveColor` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX") >** | The color when this screen is selected and active. |
| `Label` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The label of this dash screen. |
| `ScreenEnabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this dash screen is enabled or not. |
| `BaseResolution` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The resolution this screen renders at. |
| `_screenRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The root slot of this screen's visual elements. |
| `_screenCanvas` | **[Canvas](https://wiki.resonite.com/Component:Canvas "Component:Canvas")** | The canvas Component used to render this dash screen. |
| `_modalOverlayManager` | **[ModalOverlayManager](https://wiki.resonite.com/Component:ModalOverlayManager "Component:ModalOverlayManager")** | This is the Overlay manager that handles editing mode on this screen. |
| `_button` | **[RadiantDashButton](https://wiki.resonite.com/Component:RadiantDashButton "Component:RadiantDashButton")** | This is the button to switch to viewing this screen. |
| `_iconTexture` | **[Texture2D](https://wiki.resonite.com/Type:Texture2D "Type:Texture2D")** | This is the texture Component showing the icon for the tab of this screen. |
| `_closeDialog` | **[WorldCloseDialog](https://wiki.resonite.com/Component:WorldCloseDialog "Component:WorldCloseDialog")** | The close dialog this is controlling. |

Fields
Collapse

## Usage

Not used by the user, is an internally used component.

## Examples

Used for the world close dialog in the dash when closing a world.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:WorldCloseScreen&oldid=102955](https://wiki.resonite.com/index.php?title=Component:WorldCloseScreen&oldid=102955)"

Contents