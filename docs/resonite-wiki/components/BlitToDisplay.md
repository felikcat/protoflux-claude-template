# Component:BlitToDisplay

> Source: https://wiki.resonite.com/Component:BlitToDisplay

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/2/2a/BlitToDisplayComponent.png/510px-BlitToDisplayComponent.png)](https://wiki.resonite.com/File:BlitToDisplayComponent.png) **Blit To Display** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

BlitToDisplay is a component that is able to make a user's game window display a 2d texture of any kind (including render textures) and is also able to create new game windows to display images as well.

This component takes no regard for permissions at the time of writing. This component generates new windows without confirmation. New windows generated are created on new monitors or the main monitor, and are made to fit the screen.

Combining this with [Component:DisplayInfo](https://wiki.resonite.com/Component:DisplayInfo "Component:DisplayInfo") allows for getting the size of the user's screen, which can be used to adjust the texture displayed by this component to better fit the generated window.

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `TargetUser` | _direct_ **[UserRef](https://wiki.resonite.com/Type:UserRef "Type:UserRef")** | The user to display the image on their screen for. Using the local user does work. |
| `Texture` | **[ITexture](https://wiki.resonite.com/Type:ITexture "Type:ITexture")** | The texture to display to the screen. A render texture may be used here. |
| `DisplayIndex` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | which game window to display `Texture` to. If the window number doesn't exist, one is created automatically. If 0 is used, the main game window will be used. |
| `BackgroundColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color to display behind the image. |
| `FlipHorizontally` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | flip the image horizontally before displaying to the screen. |
| `FlipVertically` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | flip the image vertically before displaying to the screen. |

Fields
Collapse

## Behavior

Disabling this component does not disable its effects. Setting `TargetUser` to null does though. New windows created by this component will close the game if closed. It is unknown if this is a bug. This component can and will blind desktop users if `DisplayIndex` is set to 0 and `TargetUser` targets a desktop user.

## Examples

[989onan's](https://wiki.resonite.com/User:989onan "User:989onan") MMD player uses this to display the animated camera for the dances to the main screen.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:BlitToDisplay&oldid=93382](https://wiki.resonite.com/index.php?title=Component:BlitToDisplay&oldid=93382)"

Contents