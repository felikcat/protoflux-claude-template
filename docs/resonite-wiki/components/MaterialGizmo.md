# Component:MaterialGizmo

> Source: https://wiki.resonite.com/Component:MaterialGizmo

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/6/60/MaterialGizmoComponent.png/510px-MaterialGizmoComponent.png)](https://wiki.resonite.com/File:MaterialGizmoComponent.png) **Material Gizmo** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **MaterialGizmo** component is used to set up and manage [Material orbs](https://wiki.resonite.com/Materials "Materials") and their behavior for snapping to snapper components.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `_target` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [MaterialProvider](https://wiki.resonite.com/index.php?title=Type:MaterialProvider&action=edit&redlink=1 "Type:MaterialProvider (page does not exist)") >** | The material this Gizmo was made for. |
| `_inspectorRoot` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [Slot](https://wiki.resonite.com/Type:Slot "Type:Slot") >** | The inspector made in order to view `_target` |

Fields
Collapse

## Usage

Used with the [Material Tool](https://wiki.resonite.com/Material_Tool "Material Tool") and [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector") to manage references to materials as an item that can be held and looked at.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

have images here.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:MaterialGizmo&oldid=105326](https://wiki.resonite.com/index.php?title=Component:MaterialGizmo&oldid=105326)"

Contents