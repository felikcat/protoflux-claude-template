# Component:OpenDataFeedCategory

> Source: https://wiki.resonite.com/Component:OpenDataFeedCategory

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/1/1e/OpenDataFeedCategoryComponent.png/510px-OpenDataFeedCategoryComponent.png)](https://wiki.resonite.com/File:OpenDataFeedCategoryComponent.png) **Open Data Feed Category** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **OpenDataFeedCategory** component receives [Button Events](https://wiki.resonite.com/Button_Events "Button Events") and will open the Category with the path defined by the list `CategorySubpath`.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `View` | **[IDataFeedView](https://wiki.resonite.com/Type:IDataFeedView "Type:IDataFeedView")** | The view to change the directory for. |
| `CategorySubpath` | _direct_ **[SyncFieldList\`1](https://wiki.resonite.com/Type:SyncFieldList%601 "Type:SyncFieldList`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | A list of path directories (Like a folder path split by the slashes) to define the category to go to starting from root for `View`. |

Fields
Collapse

## Usage

Add to a slot with a button and provide a path list for this component and it will start working.

## Examples

The buttons for setting categories and menus.

## See Also

- [Data Feeds](https://wiki.resonite.com/Data_Feeds "Data Feeds")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:OpenDataFeedCategory&oldid=94954](https://wiki.resonite.com/index.php?title=Component:OpenDataFeedCategory&oldid=94954)"

Contents