# Component:GenericUserspaceDialogSpawner

> Source: https://wiki.resonite.com/Component:GenericUserspaceDialogSpawner

Collapse **Component image**

[File:GenericUserspaceDialogSpawner\`1Component.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=GenericUserspaceDialogSpawner%601Component.png "File:GenericUserspaceDialogSpawner`1Component.png") **Generic Userspace Dialog Spawner\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **GenericUserspaceDialogSpawner** only works in dash space. The Generic type it takes has to be a component type. This component activates when on the slot as a button. When activated, this component attaches a new instance of **T** to the world, triggers `Initializer` with the new Component as an argument, and then positions it in front of the user in dash space. It needs a [Component:ModalOverlayManager](https://wiki.resonite.com/Component:ModalOverlayManager "Component:ModalOverlayManager") above it in order to work.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Initializer` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") <T>** | An action that takes a Component type. |

Fields
Collapse

## See Also

- [Component:GenericModalDialogSpawner](https://wiki.resonite.com/Component:GenericModalDialogSpawner "Component:GenericModalDialogSpawner")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:GenericUserspaceDialogSpawner&oldid=96766](https://wiki.resonite.com/index.php?title=Component:GenericUserspaceDialogSpawner&oldid=96766)"

Contents