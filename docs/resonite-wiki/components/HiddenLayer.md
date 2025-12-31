# Component:HiddenLayer

> Source: https://wiki.resonite.com/Component:HiddenLayer

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/7/7e/HiddenLayerComponent.png/510px-HiddenLayerComponent.png)](https://wiki.resonite.com/File:HiddenLayerComponent.png) **Hidden Layer** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **HiddenLayer** component prevents rendering of the hierarchy it is applied to unless disabled or viewed through a camera that is explicitly set to render it. The Hidden Layer component is used for the [Dash Menu](https://wiki.resonite.com/Dash_Menu "Dash Menu")'s curved ui.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |

Fields
Collapse

## Usage

Attach to a slot which components on and below the slot should not render their visuals. The visuals will still render if viewed by a camera instructed to specifically render the hierarchy of the hidden layer.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Component:Camera](https://wiki.resonite.com/Component:Camera "Component:Camera")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:HiddenLayer&oldid=92447](https://wiki.resonite.com/index.php?title=Component:HiddenLayer&oldid=92447)"

Contents