# Component:BreadcrumbManager

> Source: https://wiki.resonite.com/Component:BreadcrumbManager

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/7/70/BreadcrumbManagerComponent.png/510px-BreadcrumbManagerComponent.png)](https://wiki.resonite.com/File:BreadcrumbManagerComponent.png) **Breadcrumb Manager** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **BreadcrumbManager** component is used to instantiate [BreadcrumbInterfaces](https://wiki.resonite.com/Component:BreadcrumbInterface "Component:BreadcrumbInterface") and remove them based on the list of path elements on a [Data Feed View Type](https://wiki.resonite.com/Type:IDataFeedView "Type:IDataFeedView").

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Path` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [SyncFieldList\`1](https://wiki.resonite.com/Type:SyncFieldList%601 "Type:SyncFieldList`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >>** | The path field in a [Data Feed View Type component](https://wiki.resonite.com/Type:IDataFeedView "Type:IDataFeedView") to show in the form of templates. |
| `UI_Root` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The place to put Breadcrumb path items in. |
| `BreadcrumbTemplate` | **[BreadcrumbInterface](https://wiki.resonite.com/Component:BreadcrumbInterface "Component:BreadcrumbInterface")** | The template to duplicate in order to create UI. |
| `SeparatorTemplate` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot to duplicate and place between elements to make them have slashes or commas between them. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| ``SetDepth:ButtonEventHandler`1<Int>`` | **[ButtonEventHandler\`1](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler%601&action=edit&redlink=1 "Type:ButtonEventHandler`1 (page does not exist)") < [Int](https://wiki.resonite.com/Type:Int "Type:Int") >** | X | Takes a number beside a button that when pressed will set the depth of the path. |
| ``SetDepth:Action`1<Int>`` | **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") < [Int](https://wiki.resonite.com/Type:Int "Type:Int") >** | X | Takes a number beside a button that when pressed will set the depth of the path. |
| `SetupTemplate:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Handles setting up a template for this component for a simple settup. |

Triggers
Collapse

## Usage

Attach to a slot and provide all fields with valid values. The manager will then allow for creating path elements automatically when navigating a data feed.

## Examples

Used heavily in the [Settings](https://wiki.resonite.com/Settings "Settings") menu to show the current path at the top.

## See Also

- [Data Feeds](https://wiki.resonite.com/Data_Feeds "Data Feeds")
- [Component:BreadcrumbInterface](https://wiki.resonite.com/Component:BreadcrumbInterface "Component:BreadcrumbInterface")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:BreadcrumbManager&oldid=98336](https://wiki.resonite.com/index.php?title=Component:BreadcrumbManager&oldid=98336)"

Contents