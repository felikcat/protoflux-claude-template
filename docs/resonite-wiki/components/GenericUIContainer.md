# Component:GenericUIContainer

> Source: https://wiki.resonite.com/Component:GenericUIContainer

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/2/24/GenericUIContainerComponent.png/510px-GenericUIContainerComponent.png)](https://wiki.resonite.com/File:GenericUIContainerComponent.png) **Generic UIContainer** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Generic UI Container** is a component that is seen on [UIX](https://wiki.resonite.com/UIX "UIX") panels and canvases. It does two primary things, match the title for the panel of a provided text, and flag when it closes and then destroys the provided hierarchy root [slot](https://wiki.resonite.com/Slot "Slot").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Title` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | Changes the title for this panel. |
| `CloseRequest` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Becomes true when this container ( [UIX](https://wiki.resonite.com/UIX "UIX") panel/canvas) is closing. |
| `CloseDestroyRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The target [slot](https://wiki.resonite.com/Slot "Slot") to destroy. |

Fields
Collapse

## Usage

There is no known usage for this component to be used in projects, but only seen on certain panels and canvases.

## Examples

The **GenericUIContainer** can be found on many default interfaces including the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector"), [Node Browser](https://wiki.resonite.com/ProtoFlux_Node_Browser "ProtoFlux Node Browser"), and [Component Inspector](https://wiki.resonite.com/index.php?title=Component_Inspector&action=edit&redlink=1 "Component Inspector (page does not exist)").

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:GenericUIContainer&oldid=94764](https://wiki.resonite.com/index.php?title=Component:GenericUIContainer&oldid=94764)"

Contents