# Component:SetDataFeedCategory

> Source: https://wiki.resonite.com/Component:SetDataFeedCategory

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/d/df/SetDataFeedCategoryComponent.png/510px-SetDataFeedCategoryComponent.png)](https://wiki.resonite.com/File:SetDataFeedCategoryComponent.png) **Set Data Feed Category** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **SetDataFeedCategory** sets the Path field for `View` when it receives a [button event](https://wiki.resonite.com/Button_Events "Button Events") from a button on the same slot or somewhere else.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `View` | **[IDataFeedView](https://wiki.resonite.com/Type:IDataFeedView "Type:IDataFeedView")** | The view to change the Path for. |
| `CategoryPath` | _direct_ **[SyncFieldList\`1](https://wiki.resonite.com/Type:SyncFieldList%601 "Type:SyncFieldList`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | What to set the path to for `View` |
| `IsInsideCategoryPath` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the View is already under `CategoryPath`. |

Fields
Collapse

## Usage

Attach to the same slot as an [IButton](https://wiki.resonite.com/Type:IButton "Type:IButton") and provide settings for this component in order for it to start working.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Data Feeds](https://wiki.resonite.com/Data_Feeds "Data Feeds")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:SetDataFeedCategory&oldid=95651](https://wiki.resonite.com/index.php?title=Component:SetDataFeedCategory&oldid=95651)"

Contents