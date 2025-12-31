# Component:WorkerInspector

> Source: https://wiki.resonite.com/Component:WorkerInspector

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/5/55/WorkerInspectorComponent.png/510px-WorkerInspectorComponent.png)](https://wiki.resonite.com/File:WorkerInspectorComponent.png) **Worker Inspector** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

A worker inspector (as opposed to [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")) is an inspector which only shows a single worker such as a component. When you grab a component reference and click Primary it will usually create one of these inspectors. You can grab sub-objects from some components which will create one of these inspectors when clicking Primary. Some workers are only obtainable via Ref Hacking which is one of the [Things to Avoid](https://wiki.resonite.com/Things_to_Avoid "Things to Avoid").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `_targetContainer` | **[Worker](https://wiki.resonite.com/index.php?title=Type:Worker&action=edit&redlink=1 "Type:Worker (page does not exist)")** | The container which holds this component or proto component (FrooxEngine.ComponentBase). |
| `_workerFilter` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[Predicate\`1](https://wiki.resonite.com/index.php?title=Type:Predicate%601&action=edit&redlink=1 "Type:Predicate`1 (page does not exist)") < [Worker](https://wiki.resonite.com/index.php?title=Type:Worker&action=edit&redlink=1 "Type:Worker (page does not exist)") >** | A filter to apply to the workers displayed. |
| `_targetWorker` | **[Worker](https://wiki.resonite.com/index.php?title=Type:Worker&action=edit&redlink=1 "Type:Worker (page does not exist)")** | The component or proto component (FrooxEngine.ComponentBase) to view. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| ``OnWorkerTypePressed:ButtonEventHandler`1<Worker>`` | **[ButtonEventHandler\`1](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler%601&action=edit&redlink=1 "Type:ButtonEventHandler`1 (page does not exist)") < [Worker](https://wiki.resonite.com/index.php?title=Type:Worker&action=edit&redlink=1 "Type:Worker (page does not exist)") >** | ✓ | Handles when the type for the worker is pressed. |
| ``OnRemoveComponentPressed:ButtonEventHandler`1<Worker>`` | **[ButtonEventHandler\`1](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler%601&action=edit&redlink=1 "Type:ButtonEventHandler`1 (page does not exist)") < [Worker](https://wiki.resonite.com/index.php?title=Type:Worker&action=edit&redlink=1 "Type:Worker (page does not exist)") >** | ✓ | Handles when the user asks to delete the viewed component or proto component (FrooxEngine.ComponentBase). |
| ``OnDuplicateComponentPressed:ButtonEventHandler`1<Worker>`` | **[ButtonEventHandler\`1](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler%601&action=edit&redlink=1 "Type:ButtonEventHandler`1 (page does not exist)") < [Worker](https://wiki.resonite.com/index.php?title=Type:Worker&action=edit&redlink=1 "Type:Worker (page does not exist)") >** | ✓ | Handles when the user asks to duplicate the viewed component or proto component (FrooxEngine.ComponentBase). |
| ``OnOpenContainerPressed:ButtonEventHandler`1<Worker>`` | **[ButtonEventHandler\`1](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler%601&action=edit&redlink=1 "Type:ButtonEventHandler`1 (page does not exist)") < [Worker](https://wiki.resonite.com/index.php?title=Type:Worker&action=edit&redlink=1 "Type:Worker (page does not exist)") >** | ✓ | Handles when the user asks to open the containing worker for the viewed component or proto component (FrooxEngine.ComponentBase). |

Triggers
Collapse

## Usage

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Examples

Is seen when viewing user or slot components, like user streams or any slot components like listed in [Components](https://wiki.resonite.com/Category:Components "Category:Components").

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:WorkerInspector&oldid=100810](https://wiki.resonite.com/index.php?title=Component:WorkerInspector&oldid=100810)"

Contents