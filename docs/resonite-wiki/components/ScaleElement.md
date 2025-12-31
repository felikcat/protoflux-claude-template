# Component:ScaleElement

> Source: https://wiki.resonite.com/Component:ScaleElement

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:ScaleElement&diff=95636) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/e/e3/ScaleElementComponent.png/510px-ScaleElementComponent.png)](https://wiki.resonite.com/File:ScaleElementComponent.png) **Scale Element** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ScaleElement** component scales itself up or down depending on if it is the selected scale element in a [Scale Group.](https://wiki.resonite.com/Component:ScaleGroup "Component:ScaleGroup").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Group` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [ScaleGroup](https://wiki.resonite.com/Component:ScaleGroup "Component:ScaleGroup") >** | The group this belongs to. If there is a group in this component's parents, the group is auto filled into this field on attach. |
| `RespondToPhysicalTouch` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to make this item selected upon physical touch. |
| `RespondToRemoteTouch` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to make this item selected upon clicking via laser. |
| `_scaleTarget` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to drive in order to influence the scale of this slot when selecting/deselecting. |

Fields
Collapse

## Usage

Used along with a [Scale Group](https://wiki.resonite.com/Component:ScaleGroup "Component:ScaleGroup") to make a list of selectable items via touching them.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Component:ScaleGroup](https://wiki.resonite.com/Component:ScaleGroup "Component:ScaleGroup")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ScaleElement&oldid=95636](https://wiki.resonite.com/index.php?title=Component:ScaleElement&oldid=95636)"

Contents