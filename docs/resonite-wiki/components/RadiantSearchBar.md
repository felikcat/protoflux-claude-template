# Component:RadiantSearchBar

> Source: https://wiki.resonite.com/Component:RadiantSearchBar

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/8/82/RadiantSearchBarComponent.png/510px-RadiantSearchBarComponent.png)](https://wiki.resonite.com/File:RadiantSearchBarComponent.png) **Radiant Search Bar** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **RadiantSearchBar** component is most commonly used and found in the [World Browser](https://wiki.resonite.com/World_Browser "World Browser").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `SearchTerm` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The term this is searching for. |
| `IsSearching` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this component is currently searching. |
| `SearchAnimTileSpeed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How fast the search animation scrolling speed should be. |
| `SearchAnimColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | What the color of the search bar should be while searching. |
| `_textField` | **[TextField](https://wiki.resonite.com/Component:TextField "Component:TextField")** | The text field for entering a search. |
| `_searchText` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [Text](https://wiki.resonite.com/Component:Text "Component:Text") >** | The text UIX Component for searching |
| `_defaultText` | **[Text](https://wiki.resonite.com/Component:Text "Component:Text")** | The text UIX Component that should be visible if a search term has not yet been entered. |
| `_searchingVisual` | **[TiledRawImage](https://wiki.resonite.com/Component:TiledRawImage "Component:TiledRawImage")** | The visual to show while searching |
| `_cancelButton` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | The button that can be used to cancel a currently running search. |
| `_defaultVisible` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | The field to drive with what should be visible by default. |
| `_searchingAnimationColor` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The field to drive for the color of the searching animation visual. |
| `_searchingTextureOffset` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The offset field to drive to create the searching animation scrolling visual. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `OnCancel:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the cancel button is touched. |

Triggers
Collapse

## Usage

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Examples

Used in the [RedX](https://wiki.resonite.com/RedX "RedX") UI.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:RadiantSearchBar&oldid=99110](https://wiki.resonite.com/index.php?title=Component:RadiantSearchBar&oldid=99110)"

Contents