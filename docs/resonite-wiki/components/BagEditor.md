# Component:BagEditor

> Source: https://wiki.resonite.com/Component:BagEditor

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:BagEditor&diff=98332) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/3/38/BagEditorComponent.png/510px-BagEditorComponent.png)](https://wiki.resonite.com/File:BagEditorComponent.png) **Bag Editor** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **BagEditor** component is a internal-use component intended to be used to generate UIX for editing an [ISyncBag](https://wiki.resonite.com/index.php?title=Type:ISyncBag&action=edit&redlink=1 "Type:ISyncBag (page does not exist)"). Some examples of Bags include the UserBag, SlotBag and WorkerBag.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `_targetBag` | **[ISyncBag](https://wiki.resonite.com/index.php?title=Type:ISyncBag&action=edit&redlink=1 "Type:ISyncBag (page does not exist)")** | The bag to edit. |
| `_addNewButton` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | Button to add a new item to the bag. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `AddNewPressed:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Handles adding new items to the bag of items. |
| `RemovePressed:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Handles removing items from the bag of items. |

Triggers
Collapse

## Usage

When `_targetBag` receives a reference to a bag, the BagEditor's slot's children will be populated with items in the bag. Each of these child slots will have the name `Element - IDXXXXXX`, where `IDXXXXX` is the [Reference ID](https://wiki.resonite.com/Type:RefID "Type:RefID") of the element. Each child slot contains a [BagEditorItem](https://wiki.resonite.com/Component:BagEditorItem "Component:BagEditorItem") component with a reference to items in the bag.

This component will misbehave when changing the `_targetBag` after it already has a reference, as doing so is unintended behavior.

This component is frequently used in conjunction with [Ref Hacking](https://wiki.resonite.com/Ref_Hacking "Ref Hacking"), as it exposes reference IDs in the element slot names.

## Examples

## See Also

- [Component:ListEditor](https://wiki.resonite.com/Component:ListEditor "Component:ListEditor")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:BagEditor&oldid=98332](https://wiki.resonite.com/index.php?title=Component:BagEditor&oldid=98332)"

Contents