# Component:GenericModalDialogSpawner

> Source: https://wiki.resonite.com/Component:GenericModalDialogSpawner

Collapse **Component image**

[File:GenericModalDialogSpawner\`1Component.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=GenericModalDialogSpawner%601Component.png "File:GenericModalDialogSpawner`1Component.png") **Generic Modal Dialog Spawner\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **GenericModalDialogSpawer** component works in world space. The Generic type it takes has to be a component type. This component activates when on the same slot as a button. When activated, this component attaches a new instance of **T** to the world, triggers `Initializer` with the new Component as an argument, and then positions it in front of the user.

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Initializer` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") <T>** | The Sync delegate to call with a |
| `Size` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The size of the dialog. |
| `CloseOnClick` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to close the Dialog on click. |
| `CloseOnContextMenu` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to close the Dialog when opening the context menu. |

Fields
Collapse

## Usage

This component needs a [Component:ModalOverlayManager](https://wiki.resonite.com/Component:ModalOverlayManager "Component:ModalOverlayManager") above it in order to work.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Component:GenericUserspaceDialogSpawner](https://wiki.resonite.com/Component:GenericUserspaceDialogSpawner "Component:GenericUserspaceDialogSpawner")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:GenericModalDialogSpawner&oldid=96767](https://wiki.resonite.com/index.php?title=Component:GenericModalDialogSpawner&oldid=96767)"

Contents