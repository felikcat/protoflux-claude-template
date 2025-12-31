# Component:Facet

> Source: https://wiki.resonite.com/Component:Facet

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/b/b6/FacetComponent.png/510px-FacetComponent.png)](https://wiki.resonite.com/File:FacetComponent.png) **Facet** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Facet** Component is the component that drives every user made [facet](https://wiki.resonite.com/Facets "Facets") in the game. This component specifically handles the sizes in which a facet can/can't, and prefers to be placed. It also reports the last size a facet was placed, the aspect ratio sizes it can be placed, and the [Canvas](https://wiki.resonite.com/Component:Canvas "Component:Canvas") that makes up the facet's contents.

When being placed into a spot, this facet finds the closest one of `PreferredSizes` that can be used while still fitting and automatically makes it the size when dropped in that spot. This only triggers if the user is just dropping it on their dash, as opposed to drag clicking the facet in.

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `MinWidth` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The minimum width this facet can be. |
| `MaxWidth` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The maximum width this facet can be. |
| `MinHeight` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The minimum height this facet can be. |
| `MaxHeight` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The maximum height this facet can be. |
| `LastPlacedSize` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2") >** | The last size that this Facet was placed as. |
| `PreferredSizes` | _direct_ **[SyncFieldList\`1](https://wiki.resonite.com/Type:SyncFieldList%601 "Type:SyncFieldList`1") < [Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2") >** | A list of sizes this canvas prefers to be placed when being dropped onto a facet holder. |
| `AllowedAspectRatios` | _direct_ **[SyncFieldList\`1](https://wiki.resonite.com/Type:SyncFieldList%601 "Type:SyncFieldList`1") < [Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2") >** | A list of allowed ratios between width and height this facet allows when being placed, lest the placement guide turns red and prevents placement. |
| `IsStandalone` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this facet has not been placed in a dash or otherwise and is out in free form space. |
| `Canvas` | **[Canvas](https://wiki.resonite.com/Component:Canvas "Component:Canvas")** | The canvas being used for the visuals of this Facet. |

Fields
Collapse

## Usage

See [Facets](https://wiki.resonite.com/Facets "Facets").

## Examples

See [Facets](https://wiki.resonite.com/Facets "Facets").

## See Also

- [Facets](https://wiki.resonite.com/Facets "Facets")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:Facet&oldid=93745](https://wiki.resonite.com/index.php?title=Component:Facet&oldid=93745)"

Contents