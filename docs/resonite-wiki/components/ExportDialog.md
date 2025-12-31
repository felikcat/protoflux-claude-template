# Component:ExportDialog

> Source: https://wiki.resonite.com/Component:ExportDialog

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/5/55/ExportDialogComponent.png/510px-ExportDialogComponent.png)](https://wiki.resonite.com/File:ExportDialogComponent.png) **Export Dialog** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

See [Exporting](https://wiki.resonite.com/Exporting "Exporting").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `SelectedExportOption` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | What Export Option is selected. |
| `ExportName` | **[TextField](https://wiki.resonite.com/Component:TextField "Component:TextField")** | The name of the Export file. |
| `_targetFolder` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The target folder location to Export to. |
| `EditEnabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this component is edit enabled. |
| `_cancel` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | The button for canceling the export. |
| `_export` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | The button to start the export. |
| `_exportOptions` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[ExportDialog.ExportOption](https://wiki.resonite.com/Component:ExportDialog#ExportOption)** | The kinds of Export options available. |
| `FileName` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [IField](https://wiki.resonite.com/Type:IField "Type:IField") >** | The name of the file when exporting. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `ExportPressed:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Exports the specified export option. |
| `CancelPressed:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Cancels the export. |

Triggers
Collapse

## Export Option

| Name | Type | Description |
| --- | --- | --- |
| `Exportable` | **[IExportable](https://wiki.resonite.com/index.php?title=Type:IExportable&action=edit&redlink=1 "Type:IExportable (page does not exist)")** | The thing to Export. Usually in [Export Category](https://wiki.resonite.com/Category:Components:Assets:Export "Category:Components:Assets:Export") |
| `ExportType` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | What kind of Export to do to the exportable. |

Fields

## Usage

See [Exporting](https://wiki.resonite.com/Exporting "Exporting").

## Examples

See [Exporting](https://wiki.resonite.com/Exporting "Exporting").

## See Also

- [Exporting](https://wiki.resonite.com/Exporting "Exporting")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ExportDialog&oldid=98446](https://wiki.resonite.com/index.php?title=Component:ExportDialog&oldid=98446)"

Contents