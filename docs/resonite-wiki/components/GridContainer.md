# Component:GridContainer

> Source: https://wiki.resonite.com/Component:GridContainer

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/1/12/GridContainerComponent.png/510px-GridContainerComponent.png)](https://wiki.resonite.com/File:GridContainerComponent.png) **Grid Container** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **GridContainer** component allows for placing facets in a grid format and storing them under a container.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `EditMode` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this grid container is currently being edited (UI edit mode) |
| `FacetsRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | Where to put facets when they are placed on the grid. |
| `_background` | **[RectTransform](https://wiki.resonite.com/Component:RectTransform "Component:RectTransform")** | The UIX rectangle that specifies what the background is. |
| `_content` | **[RectTransform](https://wiki.resonite.com/Component:RectTransform "Component:RectTransform")** | The UIX rectangle for the content like facets. |
| `_overlay` | **[RectTransform](https://wiki.resonite.com/Component:RectTransform "Component:RectTransform")** | The UIX rectangle for the grid Overlay when editing. |
| `RecalculateOnSizeChange` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to recalculate the facets on size change of the canvas. |
| `CellCount` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Int2](https://wiki.resonite.com/Type:Int2 "Type:Int2") >** | The forced cell count of this grid container. |
| `CellSize` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2") >** | How big each cell is in pixels. |
| `Padding` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | How much padding between facets there should be. |
| `_lastCalculatedCenteringOffset` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2") >** | The last centering offset calculated by this component, if at all. |
| `_lastCalculatedCellSize` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2") >** | The last cell size calculated by this component, if at all. Created when `CellCount` is specified. |
| `_lastCalculatedPadding` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2") >** | The last calculated padding between facets if at all. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `CopyFacetLayout:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Copies the facet layout to the clipboard for debugging purposes. |

Triggers
Collapse

## FacetInsertSearchDirection

| Name | Value | Description |
| --- | --- | --- |
| `Up` | 0 | Search for facet space in the Up direction. |
| `Right` | 1 | Search for facet space in the Right direction. |
| `Down` | 2 | Search for facet space in the Down direction. |
| `Left` | 3 | Search for facet space in the Left direction. |

Values

## Examples

Used in dash screens like the home tab so that facets can be placed on it during edit mode and then saved.

## See Also

- [Dash Menu](https://wiki.resonite.com/Dash_Menu "Dash Menu")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:GridContainer&oldid=98416](https://wiki.resonite.com/index.php?title=Component:GridContainer&oldid=98416)"

Contents