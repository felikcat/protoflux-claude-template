# Component:DebugFieldAdapter

> Source: https://wiki.resonite.com/Component:DebugFieldAdapter

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/e/e3/DebugFieldAdapterComponent.png/510px-DebugFieldAdapterComponent.png)](https://wiki.resonite.com/File:DebugFieldAdapterComponent.png) **Debug Field Adapter** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **DebugFieldAdapter** component just Inverts `Value`'s rgb colors and drives `Target`'s Target with it. Used with [Component:DebugFieldAdapterTest](https://wiki.resonite.com/Component:DebugFieldAdapterTest "Component:DebugFieldAdapterTest").

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This game element is a debug item. Elements like this may be removed at any time without warning, and creations should not rely on it.


## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Target` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The target field is driven to `Value`'s rgb colors inverted. |
| `Value` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The value to adapt. |

Fields
Collapse

## Usage

No need for the user to use.

## See Also

- [Component:DebugFieldAdapterTest](https://wiki.resonite.com/Component:DebugFieldAdapterTest "Component:DebugFieldAdapterTest")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:DebugFieldAdapter&oldid=96405](https://wiki.resonite.com/index.php?title=Component:DebugFieldAdapter&oldid=96405)"

Contents