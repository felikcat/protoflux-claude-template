# Component:AppEnder

> Source: https://wiki.resonite.com/Component:AppEnder

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/2/2d/AppEnderComponent.png/510px-AppEnderComponent.png)](https://wiki.resonite.com/File:AppEnderComponent.png) **App Ender** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

AppEnder is used by the local world to handle the logging out or exiting the game of the local user.

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Mode` | **[AppEnder.EndMode](https://wiki.resonite.com/Component:AppEnder#EndMode)** | Whether to exit the game or logout. |
| `ChangesSaved` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the items saved and dash changes for the current user have been saved |
| `_text` | **[TextRenderer](https://wiki.resonite.com/Component:TextRenderer "Component:TextRenderer")** | the text object that is currently showing the status of the game exiting or logging out |
| `_textColor` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | the color of the text object for this ender. |
| `_outlineColor` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The outline color of the text object for this ender. |

Fields
Collapse

## EndMode

[EndMode](https://wiki.resonite.com/Type:EndMode "Type:EndMode")

## Behavior

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AppEnder&oldid=97377](https://wiki.resonite.com/index.php?title=Component:AppEnder&oldid=97377)"

Contents