# Component:BreadcrumbInterface

> Source: https://wiki.resonite.com/Component:BreadcrumbInterface

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/e/e1/BreadcrumbInterfaceComponent.png/510px-BreadcrumbInterfaceComponent.png)](https://wiki.resonite.com/File:BreadcrumbInterfaceComponent.png) **Breadcrumb Interface** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **BreadcrumbInterface** component is used by [data feeds](https://wiki.resonite.com/Data_Feed "Data Feed") to get the translated name of one directory in a list of directories that makes a path. This is most commonly used in the [Settings](https://wiki.resonite.com/Settings "Settings") at the top to show a user where in the settings they are.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `NameConverter` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[PathSegmentConverter](https://wiki.resonite.com/index.php?title=Type:PathSegmentConverter&action=edit&redlink=1 "Type:PathSegmentConverter (page does not exist)")** | The path segment converter Sync delegate (Takes a path name and its depth) and returns a localized string. |
| `ItemName` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | The field to drive with the localized string of the path segment (on an OS, this would be like the programmer name of a folder translated to your language) |
| `PathSegment` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The path segment programmer name to convert to your language. |
| `ItemDepth` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | How many levels down in the path this string element would be. |

Fields
Collapse

## Usage

Used with a [BreadcrumbManager](https://wiki.resonite.com/Component:BreadcrumbManager "Component:BreadcrumbManager") to generate a list of path elements to show to the user in their language.

## Examples

Used in the settings header to show a user what setting they are currently viewing.

## See Also

- [Component:BreadcrumbManager](https://wiki.resonite.com/Component:BreadcrumbManager "Component:BreadcrumbManager")
- [Data Feeds](https://wiki.resonite.com/Data_Feeds "Data Feeds")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:BreadcrumbInterface&oldid=95691](https://wiki.resonite.com/index.php?title=Component:BreadcrumbInterface&oldid=95691)"

Contents