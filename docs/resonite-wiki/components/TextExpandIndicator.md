# Component:TextExpandIndicator

> Source: https://wiki.resonite.com/Component:TextExpandIndicator

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/1/1b/TextExpandIndicatorComponent.png/510px-TextExpandIndicatorComponent.png)](https://wiki.resonite.com/File:TextExpandIndicatorComponent.png) **Text Expand Indicator** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **TextExpandIndicator** component is used in inspectors to show whether or not a section like slots under another slot is expanded out and/or has any children items.

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Text` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | The text to drive with the dropdown indication. |
| `SectionRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot where children items for a slot is placed for the UI visual. |
| `ChildrenRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot to check for children slots to tell if it has children or not. |
| `Closed` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The string to display when the section is closed. |
| `Opened` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The string to display when the section is opened. |
| `Empty` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The string to display when `ChildrenRoot` is empty. |
| `CustomEmptyCheck` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[Func\`1](https://wiki.resonite.com/Type:Func%601 "Type:Func`1") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >** | A custom check sync delegate to use to check if the target is empty. |

Fields
Collapse

## Usage

This component is combined with the [Expander](https://wiki.resonite.com/Component:Expander "Component:Expander") component to show the user that the expander has expanded, collapsed, or is empty using symbols.

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:TextExpandIndicator&oldid=106588](https://wiki.resonite.com/index.php?title=Component:TextExpandIndicator&oldid=106588)"

Contents