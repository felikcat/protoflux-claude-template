# Component:LegacyWorldListManager

> Source: https://wiki.resonite.com/Component:LegacyWorldListManager

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This article describes a feature marked as legacy—this usually means there's a newer, better alternative. Legacy features might not be removed but they will not be updated, and the [team](https://wiki.resonite.com/Resonite_Team "Resonite Team") will not provide any support for them.


Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/b/b0/WorldListManagerComponent.png/510px-WorldListManagerComponent.png)](https://wiki.resonite.com/File:WorldListManagerComponent.png) **Legacy World List Manager** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **LegacyWorldListManager** component is used in the old dash to manage the world list before the [WorldsDataFeed](https://wiki.resonite.com/Component:WorldsDataFeed "Component:WorldsDataFeed") component was implemented.

![](https://wiki.resonite.com/images/c/c1/SuggestionIcon.svg)

For an up-to-date counterpart, see [Component:WorldsDataFeed](https://wiki.resonite.com/Component:WorldsDataFeed "Component:WorldsDataFeed") and read on the concept [Data Feeds](https://wiki.resonite.com/Data_Feeds "Data Feeds").


## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `UpdatingUser` | _direct_ **[UserRef](https://wiki.resonite.com/Type:UserRef "Type:UserRef")** | The user handling this component's update logic. |
| `WorldItemTemplate` | **[LegacyWorldItem](https://wiki.resonite.com/index.php?title=Type:LegacyWorldItem&action=edit&redlink=1 "Type:LegacyWorldItem (page does not exist)")** | The item Component to use as a template when making the world list. |
| `WorldItemType` | _direct_ **[SyncType](https://wiki.resonite.com/Type:SyncType "Type:SyncType")** | The C# Type of the world items. Auto filled. |
| `ShowOpenedWorlds` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Show world's that are currently open. |
| `ShowSessions` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Show sessions currently open. |
| `ShowPublishedWorlds` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Show worlds that are currently published. |
| `ShowLocallySavedWorlds` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Show locally saved worlds. |
| `MergeSessionsByWorldId` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | group sessions by world they were opened from. |
| `IdleSortDelay` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How long to wait before sorting session list while idle. |
| `InteractingSortDelay` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How long to wait before sorting session list while still interacting. |
| `SearchTerm` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The current search term for worlds. |
| `SubmittedTo` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The universe owner ID to search for worlds under (Usually G-Resonite) |
| `OnlyFeatured` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Show only featured worlds. |
| `OwnWorlds` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Show worlds made by `UpdatingUser`. |
| `ByOwner` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | Show the worlds made by this user ID. |
| `OwnerType` | **[OwnerType](https://wiki.resonite.com/Type:OwnerType "Type:OwnerType")** | The kind of entity that can own the world. |
| `MinDate` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [DateTime](https://wiki.resonite.com/Type:DateTime "Type:DateTime") >** | The minimum date for a world to show up in the results. |
| `MaxDate` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [DateTime](https://wiki.resonite.com/Type:DateTime "Type:DateTime") >** | The maximum date allowed for a world to show up in the results. |
| `MaxItems` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The maximum amount of items to show. |
| `SkipItems` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | how many starter items to skip. |
| `EmptySessions` | **[LegacyWorldListManager.EmptySessionFilter](https://wiki.resonite.com/Component:LegacyWorldListManager#EmptySessionFilter)** | How to apply filters to empty sessions. |
| `IncompatibleSessions` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to show incompatible sessions due to game version number/plugins. |
| `OnlyHeadlessHosts` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to only Show headless worlds. |
| `MinimumTotalUsers` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The minimum amount of users in order for it to show up in the list. |
| `MinimumTotalContacts` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The maximum amount of users allowed for it to show up in the list. |
| `MinSessionAccessLevel` | **[SessionAccessLevel](https://wiki.resonite.com/Type:SessionAccessLevel "Type:SessionAccessLevel")** | The minimum session access level allowed for an item to show up in the list. |
| `MaxSessionAccessLevel` | **[SessionAccessLevel](https://wiki.resonite.com/Type:SessionAccessLevel "Type:SessionAccessLevel")** | The maximum session access level allowed for an item to show up in the list. |
| `MinUptime` | **[Double](https://wiki.resonite.com/Type:Double "Type:Double")** | The minimum session access time allowed for an item to show up in the list. |
| `MaxUptime` | **[Double](https://wiki.resonite.com/Type:Double "Type:Double")** | The maximum session access time allowed for an item in the list. |
| `ParentSessionId` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The ID of the session for the user login. |
| `Visited` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >** | Whether worlds should be shown if they are either visited or not visited. |
| `SortProperties` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[LegacyWorldListManager.SortProperty](https://wiki.resonite.com/Component:LegacyWorldListManager#SortProperty)** | A list of sorting rules for the list of displayed items. |
| `IsSearching` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the component is currently doing a search. |
| `HasMoreResults` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether there is more results on other pages. |
| `TotalResults` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The total results before filtering. |
| `FilteredResults` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | How many results appeared after filtering. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `OnItemHover:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Handles when an item is hovered over in the list. |

Triggers
Collapse

## SortProperty

| Name | Type | Description |
| --- | --- | --- |
| `Parameter` | **[SortParameter](https://wiki.resonite.com/Component:LegacyWorldListManager#SortParameter)** | The sorting rule to apply |
| `Direction` | **[SortDirection](https://wiki.resonite.com/Component:LegacyWorldListManager#SortDirection)** | The direction to use when applying `Parameter` |

Fields

## SortParameter

| Name | Value | Description |
| --- | --- | --- |
| `SearchScore` | 0 | Sort by how well it matches your name search. |
| `Name` | 1 | Sort alphabetically. |
| `OpenedWorldCount` | 2 | Sort by the amount of open sessions. |
| `TotalSessionCount` | 3 | Sort by how many sessions in the past and present have been made in this world. |
| `TotalUserCount` | 4 | Sort by the total users in the world. |
| `CreationDate` | 5 | Sort by world creation daye. |
| `LastUpdateDate` | 6 | Sort by when the world was last updated by the author. |
| `FirstPublishTime` | 7 | Sort by the time the world was published to public viewing. |
| `TotalVisits` | 8 | Sort by the amount of visits by users to this world. |
| `LastVisit` | 9 | Sort by the world with the most recent visit. |
| `Random` | 10 | Sort in a random order. |

Values

## SortDirection

| Name | Value | Description |
| --- | --- | --- |
| `Ascending` | 0 | Put items in accending direction based on sort. |
| `Descending` | 1 | Put items in descending direction based on sort. |

Values

## EmptySessionFilter

| Name | Value | Description |
| --- | --- | --- |
| `HideAll` | 0 | Hide all empty sessions in the list (headless without any clients is considered empty). |
| `OnlyHeadless` | 1 | Hide only headless hosted sessions in the list. |
| `ShowAll` | 2 | Show all sessions regardless of user count. |

Values

## Usage

This is a Legacy component. Don't use.

## Examples

Used previously inside the old world list Component for the dash.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:LegacyWorldListManager&oldid=99038](https://wiki.resonite.com/index.php?title=Component:LegacyWorldListManager&oldid=99038)"

Contents