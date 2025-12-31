# Component:StorageUsageStatus

> Source: https://wiki.resonite.com/Component:StorageUsageStatus

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:StorageUsageStatus&diff=92155) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/f/f0/StorageUsageStatusComponent.png/510px-StorageUsageStatusComponent.png)](https://wiki.resonite.com/File:StorageUsageStatusComponent.png) **Storage Usage Status** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

Storage Usage Status is a component that is used to read how much storage a user has used, total, shared, and that has left to share.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `OwnerId` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The id of the user this is reading data from |
| `GroupMemberQuota` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to read group storage limits. |
| `HasValidData` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this component has successfully grabbed the data. |
| `StorageBytes` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Long](https://wiki.resonite.com/Type:Long "Type:Long")** | how many bytes of storage `OwnerId` has total |
| `FullStorageBytes` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Long](https://wiki.resonite.com/Type:Long "Type:Long")** | how many bytes of storage `OwnerId` has used currently. |
| `ShareableStorageBytes` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Long](https://wiki.resonite.com/Type:Long "Type:Long")** | How many bytes of storage `OwnerId` currently has ready to share. |
| `SharedStorageBytes` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Long](https://wiki.resonite.com/Type:Long "Type:Long")** | How many bytes of storage `OwnerId` has shared with others currently. |
| `UsageBytes` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Long](https://wiki.resonite.com/Type:Long "Type:Long")** | The total amount of bytes being used by `OwnerId`. |
| `UsageRatio` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | the percentage of how full `OwnerId`'s storage is from 0->1 |
| `StorageString` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | String version with nice formatting applied of how much storage `OwnerId` has. |
| `FullStorageString` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | String version with nice formatting applied of |
| `ShareableStorageString` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | String version with nice formatting applied of how much storage `OwnerId` has ready to share. |
| `SharedStorageString` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | String version with nice formatting applied of how much storage `OwnerId` has shared with others. |
| `UsageString` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | String version with nice formatting applied of how much storage `OwnerId` has used. |
| `RatioString` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | String version with nice formatting applied of how full `OwnerId`'s storage is. |

Fields
Collapse

## Usage

Can only be used in user space (verify?)

## Examples

Used in the cloud storage facets to show the user how much storage they have left.

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:StorageUsageStatus&oldid=92155](https://wiki.resonite.com/index.php?title=Component:StorageUsageStatus&oldid=92155)"

Contents