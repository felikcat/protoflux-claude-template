# Component:SlotInspector

> Source: https://wiki.resonite.com/Component:SlotInspector

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/3/30/SlotInspectorComponent.png/510px-SlotInspectorComponent.png)](https://wiki.resonite.com/File:SlotInspectorComponent.png) **Slot Inspector** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Slot Inspector** component controls the slot items shown in a [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector") and their drop down menus.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `_selectionReference` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [SyncRef\`1](https://wiki.resonite.com/Type:SyncRef%601 "Type:SyncRef`1") < [Slot](https://wiki.resonite.com/Type:Slot "Type:Slot") >>** | The slot this points to. |
| `_rootSlot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The root of the visual for this item. |
| `_childContainer` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The container for slot inspectors that are children of this one. |
| `_depth` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | How far down this slot inspector is from the root selected slot inspector in it's parent [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector"). |
| `_expander` | **[Expander](https://wiki.resonite.com/Component:Expander "Component:Expander")** | The component responsible for expanding the children slot inspector hierarchy of this item. |
| `_expanderIndicator` | **[TextExpandIndicator](https://wiki.resonite.com/Component:TextExpandIndicator "Component:TextExpandIndicator")** | The indicator for whether the slot inspector children hierarchy is expanded or not. |
| `_slotNameText` | **[Text](https://wiki.resonite.com/Component:Text "Component:Text")** | The name of the slot this slot inspector is pointing to. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| ``IsTargetEmpty:Func`1<Bool>`` | **[Func\`1](https://wiki.resonite.com/Type:Func%601 "Type:Func`1") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >** | ✓ | When called, returns if the target slot contains no children slots. |

Triggers
Collapse

## Usage

Not used directly by the user. Used in [Scene Inspectors](https://wiki.resonite.com/index.php?title=Scene_Inspectors&action=edit&redlink=1 "Scene Inspectors (page does not exist)").

## Examples

Used in [Scene Inspectors](https://wiki.resonite.com/index.php?title=Scene_Inspectors&action=edit&redlink=1 "Scene Inspectors (page does not exist)").

## See Also

- [Scene Inspectors](https://wiki.resonite.com/index.php?title=Scene_Inspectors&action=edit&redlink=1 "Scene Inspectors (page does not exist)")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:SlotInspector&oldid=99371](https://wiki.resonite.com/index.php?title=Component:SlotInspector&oldid=99371)"

Contents