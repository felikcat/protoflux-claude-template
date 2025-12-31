# Component:LightIntensityFieldAdapter

> Source: https://wiki.resonite.com/Component:LightIntensityFieldAdapter

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This article describes a feature marked as legacy—this usually means there's a newer, better alternative. Legacy features might not be removed but they will not be updated, and the [team](https://wiki.resonite.com/Resonite_Team "Resonite Team") will not provide any support for them.


Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/5/54/LightIntensityFieldAdapterComponent.png/510px-LightIntensityFieldAdapterComponent.png)](https://wiki.resonite.com/File:LightIntensityFieldAdapterComponent.png) **Light Intensity Field Adapter** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Light Intensity Field Adapter** component is used to convert the light intensity from migrated content to the new color space system.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Target` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The light intensity field to drive. |
| `Value` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The original value in which to convert. |
| `Profile` | **[ColorProfile](https://wiki.resonite.com/Type:ColorProfile "Type:ColorProfile")** | Which color profile to convert to when converting `Value`. |

Fields
Collapse

## Usage

Do not use in new content.

## Examples

Used in legacy content to convert old lights to the new color system.

## See Also

- [Component:Light](https://wiki.resonite.com/Component:Light "Component:Light")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:LightIntensityFieldAdapter&oldid=103807](https://wiki.resonite.com/index.php?title=Component:LightIntensityFieldAdapter&oldid=103807)"

Contents