# Component:AccountMigrationStatus

> Source: https://wiki.resonite.com/Component:AccountMigrationStatus

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/7/7d/AccountMigrationStatusComponent.png/510px-AccountMigrationStatusComponent.png)](https://wiki.resonite.com/File:AccountMigrationStatusComponent.png) **Account Migration Status** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

This component is able to take a taskID of a migration on the cloud, and is able to display the information about said Migration. This info is grabbed from a AccountMigrationTask object internally which is returned by the SkyFrost API.

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `TaskId` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | A UUID of a task that has been done, waiting, or is being done on the SkyFrost cloud. |
| `Exists` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether `TaskId` is a valid ID for a task on the cloud |
| `Name` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The name of the found migration task. |
| `Description` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The description of the task. Usually starts with "Account Migration" or "Favorites migration" |
| `State` | **[MigrationState](https://wiki.resonite.com/Type:MigrationState "Type:MigrationState")** | Also known as "Status", this will show whether the task has started, and if it's done or currently running. |
| `EstimatedQueuePosition` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Int](https://wiki.resonite.com/Type:Int "Type:Int") >** | An estimate of the migration task's position on the list of migrations the SkyFrost servers are currently doing. This number can be high if a huge influx of migrations is happening at the current time. |
| `StartCount` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Usually 1 for some reason <br>_This article or section is a stub. You can help the Resonite wiki by expanding it._ |
| `CreatedOn` | **[DateTime](https://wiki.resonite.com/Type:DateTime "Type:DateTime")** | When the migration task was submitted to the list of migrations to be done on the cloud |
| `StartedOn` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [DateTime](https://wiki.resonite.com/Type:DateTime "Type:DateTime") >** | When the cloud started to migrate the items for this task. |
| `CompletedOn` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [DateTime](https://wiki.resonite.com/Type:DateTime "Type:DateTime") >** | When the Cloud completed this migration task. |
| `RecordsPerMinute` | **[Double](https://wiki.resonite.com/Type:Double "Type:Double")** | A calculation average of how fast the SkyFrost cloud is transfering items from the source platform to Resonite. |
| `CurrentlyMigrating` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | What type of thing the cloud is currently migrating? |
| `CurrentItem` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | What item the cloud is currently migrating for this task. |
| `TotalRecordCount` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | How many records this migration task is to migrate in total. |
| `TotalMigratedRecordCount` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | How many records this migration has successfully migrated so far. |
| `TotalFailedRecordCount` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | How many records this migration failed to migrate. |
| `TotalMigratedVariableCount` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | How many Cloud Variables that the user has created themselves that this migration task has to migrate in total. |
| `TotalMigratedVariableDefinitionCount` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | How many Cloud Variable Definitions this migration task has to migrate in total. |
| `TotalContactCount` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | How many friend connections that this migration task has to migrate in total. |
| `MigratedContactCount` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | How many friend connections that this migration task has migrated so far. |
| `MigratedMessageCount` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | How many messages sent by the user that this migration task has migrated so far. |
| `TotalGroupCount` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | How many groups that the user has created that this migration task has to migrate in total. |
| `MigratedGroupCount` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | How many groups that the user has created that the migration task has migrated so far. |
| `TotalMigratedMemberCount` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | How many member names of groups that the user has created has been migrated by the migration task. |

Fields
Collapse

## Behavior

does not work outside of user space.

## Examples

Used inside of the migration panel tab

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AccountMigrationStatus&oldid=91004](https://wiki.resonite.com/index.php?title=Component:AccountMigrationStatus&oldid=91004)"

Contents