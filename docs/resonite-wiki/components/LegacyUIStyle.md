# Component:LegacyUIStyle

> Source: https://wiki.resonite.com/Component:LegacyUIStyle

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This article describes a feature marked as legacy—this usually means there's a newer, better alternative. Legacy features might not be removed but they will not be updated, and the [team](https://wiki.resonite.com/Resonite_Team "Resonite Team") will not provide any support for them.


Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/8/89/LegacyUIStyleComponent.png/510px-LegacyUIStyleComponent.png)](https://wiki.resonite.com/File:LegacyUIStyleComponent.png) **LegacyUIStyle** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **LegacyUIStyle** component is used in older content to specify what colors a UI should be depending on where it is. This should not be used in new content, and should be removed/replaced whenever possible.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Color` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The normal color. |
| `UserParentedColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color a UI should have when parented under the user. |
| `PrivateColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color a UI should have when it's in [userspace](https://wiki.resonite.com/Userspace "Userspace"). |

Fields
Collapse

## Examples

Used to specify to Legacy UI what color it should use.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:LegacyUIStyle&oldid=100111](https://wiki.resonite.com/index.php?title=Component:LegacyUIStyle&oldid=100111)"

Contents