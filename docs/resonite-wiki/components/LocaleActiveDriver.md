# Component:LocaleActiveDriver

> Source: https://wiki.resonite.com/Component:LocaleActiveDriver

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/4/46/LocaleActiveDriverComponent.png/510px-LocaleActiveDriverComponent.png)](https://wiki.resonite.com/File:LocaleActiveDriverComponent.png) **Locale Active Driver** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **LocaleActiveDriver** does a comparison against the local user's locale code and returns if it matches.

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Target` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | The field to drive with whether or not `LocaleCode` is the local user's active locale code. |
| `LocaleCode` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The locale code to check for ignoring cass. |
| `MatchMainLanguage` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to match to the locale's main language. |

Fields
Collapse

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:LocaleActiveDriver&oldid=94876](https://wiki.resonite.com/index.php?title=Component:LocaleActiveDriver&oldid=94876)"

Contents