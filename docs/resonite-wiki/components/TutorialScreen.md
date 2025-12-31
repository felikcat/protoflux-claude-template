# Component:TutorialScreen

> Source: https://wiki.resonite.com/Component:TutorialScreen

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/0/0e/TutorialScreenComponent.png/510px-TutorialScreenComponent.png)](https://wiki.resonite.com/File:TutorialScreenComponent.png) **Tutorial Screen** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **TutorialScreen** component controls a screen prompting the user to go through the tutorial in their dash.

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
| `_swapRegion` | **[SlideSwapRegion](https://wiki.resonite.com/Component:SlideSwapRegion "Component:SlideSwapRegion")** | This is the swap region used to show the screen and slide it away/in when it is switched from/to. |
| `_currentScreen` | **[TutorialScreen.Screen](https://wiki.resonite.com/Component:TutorialScreen#Screen)** | The current screen this tutorial screen dialog is showing. |
| `_heightField` | **[QuantityTextEditorParser\`2](https://wiki.resonite.com/Component:QuantityTextEditorParser%602 "Component:QuantityTextEditorParser`2") < [Distance](https://wiki.resonite.com/Type:Distance "Type:Distance"), [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | The field used to enter in and store the user's height setting. |
| `_nextEnabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the next button is enabled or not so the user can continue. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `OnNext:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Handles when the next screen button is enabled. |
| `OnCreateAccount:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Handles when the user asks to create an account. |
| `OnLoginAccount:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Handles when the user logs into an account. |
| `OnSkipAccount:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Handles when the user skips setting up an account. |
| `OnStartTutorial:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Handles when the user asks to start the tutorial world. |

Triggers
Collapse

## Screen

| Name | Value | Description |
| --- | --- | --- |
| `Welcome` | 0 | Screen is currently showing the welcome to resonite screen. |
| `Language` | 1 | Screen is currently showing the select your language screen. |
| `Audio` | 2 | Screen is currently showing the select audio devices screen. |
| `BasicSettings` | 3 | Screen is currently showing the basic settings screen. |
| `Account` | 4 | Screen is currently showing the create or skip creating account screen. |
| `StartTutorial` | 5 | Screen is currently showing the start tutorial screen. |

Values

## Usage

## Examples

Used to show the tutorial screen in the dash when the user starts the game for the first time (or wipes their cache)

## See Also

- [Tutorial](https://wiki.resonite.com/index.php?title=Tutorial&action=edit&redlink=1 "Tutorial (page does not exist)")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:TutorialScreen&oldid=100745](https://wiki.resonite.com/index.php?title=Component:TutorialScreen&oldid=100745)"

Contents