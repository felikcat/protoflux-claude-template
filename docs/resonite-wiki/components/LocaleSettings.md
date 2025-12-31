# Component:LocaleSettings

> Source: https://wiki.resonite.com/Component:LocaleSettings

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/6/63/LocaleSettingsComponent.png/510px-LocaleSettingsComponent.png)](https://wiki.resonite.com/File:LocaleSettingsComponent.png) **Locale Settings** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Locale Settings** component is part of the [Settings](https://wiki.resonite.com/Settings "Settings") system and controls the platform's language.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `PrimaryInterfaceLocaleCode` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The primary language for the UI. |
| `CultureLocaleCode` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The locale code for the primary language, Ex: "en\_us", "ru", or "pl\_PL" |
| `UseImperialUnits` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to use Imperial or Metric units regardless of language selection. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| ``SetCurrentLocale:Action`1<String>`` | **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | X | Called when the set current locale button is touched. |

Triggers
Collapse

## Usage

Not used directly by the user.

## Examples

Used in the [Settings](https://wiki.resonite.com/Settings "Settings") menu.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:LocaleSettings&oldid=103811](https://wiki.resonite.com/index.php?title=Component:LocaleSettings&oldid=103811)"

Contents