# Component:MigrationDialog

> Source: https://wiki.resonite.com/Component:MigrationDialog

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This is a **[userspace](https://wiki.resonite.com/Userspace "Userspace") component** — you cannot attach it anywhere but the userspace. Messing with the userspace can be fun, but it is **not recommended** as you risk messing your dash up if you don't know what you're doing.


Collapse **Component image**

[File:MigrationDialogComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=MigrationDialogComponent.png "File:MigrationDialogComponent.png") **Migration Dialog** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **MigrationDialog** component is used to collect information on what migration action should be done for transfering content from other platforms or other Resonite accounts.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `_usernameField` | **[TextField](https://wiki.resonite.com/Component:TextField "Component:TextField")** | The username of the account to transfer from. |
| `_passwordField` | **[TextField](https://wiki.resonite.com/Component:TextField "Component:TextField")** | The password of the account to transfer from. |
| `_migrateFavorites` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to migrate favorites from the account or not. |
| `_overwriteFavorites` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to replace the favorites on the currently logged in account with the transfering from account. |
| `_preserveOldHome` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to keep the home world setting from the other account or create a new default home. |
| `_migrateContacts` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to migrate contacts from the account or not. |
| `_migrateMessageHistory` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to migrate message history from the account or not. |
| `_migrateRecords` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to migrate items, worlds, avatars, message items, or other objects/data from the account or not. |
| `_migrateCloudVariables` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to migrate cloud variables made by the account or not. |
| `_migratedCloudVariableDefinitions` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to migrate values defined for other user's variables from the account or not. |
| `_migrateGroups` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to migrate groups from the account or not. |
| `_groupsRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The root of the groups section. |
| `_groupsMessage` | **[Text](https://wiki.resonite.com/Component:Text "Component:Text")** | The text element for groups dialog. |
| `_loadGroupsButton` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | The button for loading groups in. |
| `CurrentState` | **[MigrationDialog.State](https://wiki.resonite.com/Component:MigrationDialog#State)** | The current state of the migration dialog visual. |
| `_swapRegion` | **[SlideSwapRegion](https://wiki.resonite.com/Component:SlideSwapRegion "Component:SlideSwapRegion")** | Thw region used for animation when switching between different screens in the migration dialog |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| ``SetOverwrite:ButtonEventHandler`1<Bool>`` | **[ButtonEventHandler\`1](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler%601&action=edit&redlink=1 "Type:ButtonEventHandler`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >** | ✓ | Called when the overwrite button is touched. |
| ``SetPreserveHome:ButtonEventHandler`1<Bool>`` | **[ButtonEventHandler\`1](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler%601&action=edit&redlink=1 "Type:ButtonEventHandler`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >** | ✓ | Called when the preserve home button is touched. |
| `ChooseAllData:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the choose all data button is touched. |
| ``ChangeStep:ButtonEventHandler`1<MigrationDialog.State>`` | **[ButtonEventHandler\`1](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler%601&action=edit&redlink=1 "Type:ButtonEventHandler`1 (page does not exist)") < [MigrationDialog.State](https://wiki.resonite.com/Component:MigrationDialog#State) >** | ✓ | Called when the change step button is touched. |
| ``SaveGroupSelectionAndChange:ButtonEventHandler`1<MigrationDialog.State>`` | **[ButtonEventHandler\`1](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler%601&action=edit&redlink=1 "Type:ButtonEventHandler`1 (page does not exist)") < [MigrationDialog.State](https://wiki.resonite.com/Component:MigrationDialog#State) >** | ✓ | Called when the save group selection and change button is touched. |
| ``CheckLoginAndNext:ButtonEventHandler`1<MigrationDialog.State>`` | **[ButtonEventHandler\`1](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler%601&action=edit&redlink=1 "Type:ButtonEventHandler`1 (page does not exist)") < [MigrationDialog.State](https://wiki.resonite.com/Component:MigrationDialog#State) >** | ✓ | Called when the Check login and next button is touched. |
| `LoadGroupsPressed:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the load groups button is touched. |
| ``OnSourceSelected:ButtonEventHandler`1<String>`` | **[ButtonEventHandler\`1](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler%601&action=edit&redlink=1 "Type:ButtonEventHandler`1 (page does not exist)") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | ✓ | Called when the source button is touched. |
| `StartMigrationPressed:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the start migration button is touched. |
| `CancelPressed:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the cancel button is touched. |

Triggers
Collapse

## State

| Name | Value | Description |
| --- | --- | --- |
| `Source` | 0 | The user is choosing the source like resonite or older platforms. |
| `Account` | 1 | The user is specifying the account details of the account to transfer from. |
| `MigrationType` | 2 | The user is choosing the migration type. |
| `ChooseData` | 3 | The user is choosing what data to move. |
| `ChooseGroups` | 4 | The user is choosing what groups to move. |
| `ChooseOverwrite` | 5 | The user is choosing any overwriting options. |
| `ChooseHome` | 6 | The user is picking Whether to transfer the source account's home world or generate a new one from default. |
| `ConfirmStart` | 7 | The user is on the screen to confirm to start the migration. |

Values

## Usage

Use internally, do not use.

## Examples

Migration screen.

## See Also

- [Migration](https://wiki.resonite.com/index.php?title=Migration&action=edit&redlink=1 "Migration (page does not exist)")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:MigrationDialog&oldid=105332](https://wiki.resonite.com/index.php?title=Component:MigrationDialog&oldid=105332)"

Contents