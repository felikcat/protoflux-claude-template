# Component:PagingControl

> Source: https://wiki.resonite.com/Component:PagingControl

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:PagingControl&diff=98784) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/c/c5/PagingControlComponent.png/510px-PagingControlComponent.png)](https://wiki.resonite.com/File:PagingControlComponent.png) **Paging Control** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **PagingControl** component allows for counting up a number of items specified, then outputs it to either a [Text](https://wiki.resonite.com/Component:Text "Component:Text") or [TextRenderer](https://wiki.resonite.com/Component:TextRenderer "Component:TextRenderer") component.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `ItemsPerPage` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The increment to count up by. |
| `TotalItems` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The total amount of items. |
| `HasMoreItems` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Allows to count beyond the max set of items. |
| `SkipItems` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Skips items that are listed here. |
| `NoItemsLabel` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | Shows the output as this when there are no items. |
| `PagingInfoLabel` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The structure of how the items will be shown to the user. |
| `TotalPages` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The total amount of items. |
| `RemainingItems` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Shows how many items are remaining. |
| `_label` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | The text to output. |
| `_previousEnabled` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Becomes false if the minimum is currently reached. |
| `_nextEnabled` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Becomes false if the maximum is currently reached. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `NextPage:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Switches to the next page via button. |
| `PreviousPage:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Switches to the previous page via button. |
| `NextPage:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Switches to the next page via action. |
| `PreviousPage:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Switches to the previous page via action. |

Triggers
Collapse

## Usage

Great for counting items, and for controlling UI that can switch pages.

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:PagingControl&oldid=98784](https://wiki.resonite.com/index.php?title=Component:PagingControl&oldid=98784)"

Contents