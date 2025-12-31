# Component:ListEditor

> Source: https://wiki.resonite.com/Component:ListEditor

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/c/c8/ListEditorComponent.png/510px-ListEditorComponent.png)](https://wiki.resonite.com/File:ListEditorComponent.png) **List Editor** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ListEditor** component is a internal-use component intended to be used to generate UIX for editing an [ISyncList](https://wiki.resonite.com/index.php?title=Type:ISyncBag&action=edit&redlink=1 "Type:ISyncBag (page does not exist)").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `_targetList` | **[ISyncList](https://wiki.resonite.com/Type:ISyncList "Type:ISyncList")** | The list to edit. |
| `_addNewButton` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | Button to add a new item to the list. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `AddNewPressed:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the add new item button is touched. |
| `MoveUpPressed:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the move item up button is touched. |
| `MoveDownPressed:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the move item down button is touched. |
| `RemovePressed:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the remove item button is touched. |

Triggers
Collapse

## Usage

When `_targetList` receives a reference to a list, the ListEditor's slot's children will be populated with items in the list. Each of these child slots will have the name `Element`. Each slot contains a [HorizontalLayout](https://wiki.resonite.com/Component:HorizontalLayout "Component:HorizontalLayout") component and [RectTransform](https://wiki.resonite.com/Component:RectTransform "Component:RectTransform") component.

This component will misbehave when changing the `_targetList` after it already has a reference, as doing so is unintended behavior.

This component is much less useful than its cousin, [BagEditor](https://wiki.resonite.com/Component:BagEditor "Component:BagEditor"), as it does not expose any method to reference the list members from in-game. FrooxEngine uses internal code to add references on child slots of the elements when building the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector") UI.

## Examples

## See Also

- [Component:BagEditor](https://wiki.resonite.com/Component:BagEditor "Component:BagEditor")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ListEditor&oldid=99063](https://wiki.resonite.com/index.php?title=Component:ListEditor&oldid=99063)"

Contents