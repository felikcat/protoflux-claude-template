# Component:AccountMigrationsList

> Source: https://wiki.resonite.com/Component:AccountMigrationsList

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/d/d0/AccountMigrationsListComponent.png/510px-AccountMigrationsListComponent.png)](https://wiki.resonite.com/File:AccountMigrationsListComponent.png) **Account Migrations List** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

Account Migrations List is a component that only works in user space. It checks the current Migrations being ran by the cloud and gives a running count every game update. It shows how many there are total including counts of different statuses the different migrations have.

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `TotalMigrations` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | How many total migrations are currently happening on the cloud right now for the current user. |
| `WaitingMigrations` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | How many migrations are currently waiting to start on the cloud right now for the current user. |
| `RunningMigrations` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | How many migrations are currently happening on the cloud right now for the current user. |
| `CompletedMigrations` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | How many completed migrations have happened on the cloud before for the current user. |
| `MigrationTaskIds` | _direct_ **[SyncFieldList\`1](https://wiki.resonite.com/Type:SyncFieldList%601 "Type:SyncFieldList`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | The task ID's of all the migrations for the current user. |

Fields
Collapse

## Behavior

Only works in user space. Updates with migrations automatically.

## Examples

Possibly used in the migrations tab to show the user what migrations they have done or are doing (CONFIRM?)

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AccountMigrationsList&oldid=91003](https://wiki.resonite.com/index.php?title=Component:AccountMigrationsList&oldid=91003)"

Contents