# Component:SceneInspector

> Source: https://wiki.resonite.com/Component:SceneInspector

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/8/86/SceneInspectorComponent.png/510px-SceneInspectorComponent.png)](https://wiki.resonite.com/File:SceneInspectorComponent.png) **Scene Inspector** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

See [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")!

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Root` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [Slot](https://wiki.resonite.com/Type:Slot "Type:Slot") >** | The root of the view of this inspector's hiearchy. |
| `ComponentView` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The currently selected slot to view components for. |
| `_rootText` | **[Sync\`1](https://wiki.resonite.com/Type:Sync%601 "Type:Sync`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | The text field for the display of the root hiearchy slot for this inspector's view. |
| `_componentText` | **[Sync\`1](https://wiki.resonite.com/Type:Sync%601 "Type:Sync`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | The text field for the display of the slot for this inspector's component view. |
| `_hierarchyContentRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The root of the view for slots on the currently viewed slot hiearchy. |
| `_componentsContentRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The root of the view for components on the currently selected slot. |
| `_currentComponent` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The current component this is looking at. |
| `_currentRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The current root this is looking at. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `OnRootUpPressed:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the go up in hiearchy button is touched. |
| `OnObjectRootPressed:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the view slot component list button is touched. |
| `OnSetRootPressed:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the set root slot view button is touched. |
| `OnAddChildPressed:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the add child button is touched. |
| `OnInsertParentPressed:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the insert parent button is touched. |
| `OnAttachComponentPressed:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the attach component dialog button is touched. |
| ``OnComponentSelected:Action`2<ComponentSelector, Type>`` | **[Action\`2](https://wiki.resonite.com/index.php?title=Type:Action%602&action=edit&redlink=1 "Type:Action`2 (page does not exist)") < [ComponentSelector](https://wiki.resonite.com/Component:ComponentSelector "Component:ComponentSelector"), [Type](https://wiki.resonite.com/Type:Type "Type:Type") >** | ✓ | Handles when a component selector is told to attach a component to the slot this is on. |
| `OnDestroyPressed:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the destroy button is touched. |
| `OnDestroyPreservingAssetsPressed:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the recycle button is touched. |
| `OnDuplicatePressed:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the button is touched. |

Triggers
Collapse

## Usage

See [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")!

## Examples

See [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")!

## See Also

- [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:SceneInspector&oldid=99166](https://wiki.resonite.com/index.php?title=Component:SceneInspector&oldid=99166)"

Contents