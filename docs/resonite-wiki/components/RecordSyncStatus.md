# Component:RecordSyncStatus

> Source: https://wiki.resonite.com/Component:RecordSyncStatus

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:RecordSyncStatus&diff=95469) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/7/79/RecordSyncStatusComponent.png/510px-RecordSyncStatusComponent.png)](https://wiki.resonite.com/File:RecordSyncStatusComponent.png) **Record Sync Status** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **RecordSyncStatus** component reports the current status of syncing items like worlds, avatars, settings, and user generated content when present in the user space world where the dash is.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `RecordQueueCount` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | How many items are left in the queue of items to Sync from the user's machine to the cloud. |
| `AssetVariantQueueCount` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | How many asset variants are left to upload for the items being uploaded to the cloud. |
| `CurrentTaskProgress` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How far along the Asset uploader is to uploading the current item. |
| `LastError` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | The last error given by the cloud item uploader process. |
| `StatusMessage` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | The status message for the item uploader process. |
| `FullySyncedColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color the UI should be if it is fully done syncing. |
| `ErrorColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color the UI should be if there was an error (UH OH!!! [Stuck Sync](https://wiki.resonite.com/Stuck_Sync "Stuck Sync")!!!) |
| `SyncingRecordsColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color the UI should be when the item uploader task is syncing Record items. |
| `UploadingAssetVariantsColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color the UI should be when the item uploader is uploading Asset variants for things like textures or skyboxes. |

Fields
Collapse

## Usage

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Examples

Used in the user dash to show syncing status at the top.

## See Also

- [Stuck Sync](https://wiki.resonite.com/Stuck_Sync "Stuck Sync")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:RecordSyncStatus&oldid=95469](https://wiki.resonite.com/index.php?title=Component:RecordSyncStatus&oldid=95469)"

Contents