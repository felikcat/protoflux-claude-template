# Component:LegacySwapCanvasPanel

> Source: https://wiki.resonite.com/Component:LegacySwapCanvasPanel

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This article describes a feature marked as legacy—this usually means there's a newer, better alternative. Legacy features might not be removed but they will not be updated, and the [team](https://wiki.resonite.com/Resonite_Team "Resonite Team") will not provide any support for them.


Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/8/89/LegacySwapCanvasPanelComponent.png/510px-LegacySwapCanvasPanelComponent.png)](https://wiki.resonite.com/File:LegacySwapCanvasPanelComponent.png) **Legacy Swap Canvas Panel** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **LegacySwapCanvasPanel** was used to swap between different panels using some buttons.

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `_canvas` | **[Canvas](https://wiki.resonite.com/Component:Canvas "Component:Canvas")** | The canvas that contains the entire swap visual. |
| `_panel` | **[LegacyPanel](https://wiki.resonite.com/Component:LegacyPanel "Component:LegacyPanel")** | The panel that contains the entire swap panel. |
| `_currentPanel` | **[RectTransform](https://wiki.resonite.com/Component:RectTransform "Component:RectTransform")** | The current panel visual this is switched to. |
| `_container` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot that contains the visuals for the swap panel. |

Fields
Collapse

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:LegacySwapCanvasPanel&oldid=99184](https://wiki.resonite.com/index.php?title=Component:LegacySwapCanvasPanel&oldid=99184)"

Contents