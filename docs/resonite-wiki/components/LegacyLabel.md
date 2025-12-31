# Component:LegacyLabel

> Source: https://wiki.resonite.com/Component:LegacyLabel

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This article describes a feature marked as legacy—this usually means there's a newer, better alternative. Legacy features might not be removed but they will not be updated, and the [team](https://wiki.resonite.com/Resonite_Team "Resonite Team") will not provide any support for them.


Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/8/84/LegacyLabelComponent.png/510px-LegacyLabelComponent.png)](https://wiki.resonite.com/File:LegacyLabelComponent.png) **Legacy Label** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **LegacyLabel** component is a leftover Component from content migrated from other platforms. It should not be used, and should be replaced whenever possible.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `TextRenderer` | **[TextRenderer](https://wiki.resonite.com/Component:TextRenderer "Component:TextRenderer")** | The text renderer for the label visual. |
| `BaseColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The base color of the label visual. |
| `BaseColorElement` | **[ILegacyUIElement](https://wiki.resonite.com/index.php?title=Type:ILegacyUIElement&action=edit&redlink=1 "Type:ILegacyUIElement (page does not exist)")** | The UI element for the base color. |
| `Brightness` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The brightness of the label visual. |
| `LerpRatio` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | A value from 0<->1 to lerp `BaseColor` and `LerpColor` with. |
| `LerpColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color to lerp to. |
| `_textColor` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The field to drive with a color between `BaseColor` and `LerpColor` using `LerpRatio` as the specifier for the in between color. |

Fields
Collapse

## Usage

Not to be used by the user, legacy content.

## Examples

Used in legacy content.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:LegacyLabel&oldid=99021](https://wiki.resonite.com/index.php?title=Component:LegacyLabel&oldid=99021)"

Contents