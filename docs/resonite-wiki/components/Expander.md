# Component:Expander

> Source: https://wiki.resonite.com/Component:Expander

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:Expander&diff=88658) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/f/fd/ExpanderComponent.png/510px-ExpanderComponent.png)](https://wiki.resonite.com/File:ExpanderComponent.png) **Expander** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Expander** component is an intractable [UIX](https://wiki.resonite.com/UIX "UIX") element that expands a section called the `SectionRoot` under itself. The `SectionRoot`'s active state will toggle when that expander is triggered, expanding it under the [Slot](https://wiki.resonite.com/Slot "Slot") the expander is on. This can be seen on the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector").

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `SectionRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot to expend with, by activating the slot that is referenced when toggled. |

Fields
Collapse

## Usage

This component is combined with the [Button](https://wiki.resonite.com/Component:Button "Component:Button") component to trigger this expander component. This component is also combined with the [TextExpandIndicator](https://wiki.resonite.com/Component:TextExpandIndicator "Component:TextExpandIndicator") component to drive the text and show the user that this expander has expanded, collapsed, or is empty.

## Examples

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:Expander&oldid=88658](https://wiki.resonite.com/index.php?title=Component:Expander&oldid=88658)"

Contents