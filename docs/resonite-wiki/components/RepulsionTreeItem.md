# Component:RepulsionTreeItem

> Source: https://wiki.resonite.com/Component:RepulsionTreeItem

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/f/f8/RepulsionTreeItemComponent.png/510px-RepulsionTreeItemComponent.png)](https://wiki.resonite.com/File:RepulsionTreeItemComponent.png) **Repulsion Tree Item** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Repulsion tree item is used along side the [Repulsion Tree Simulator Component](https://wiki.resonite.com/Component:RepulsionTreeSimulator "Component:RepulsionTreeSimulator") to make a live repulsion tree simulation. Check the simulator's page for a more detailed explanation.

![](https://wiki.resonite.com/images/b/b7/DangerIcon.svg)

This does lots of writes to every slot under it, this is experimental and users should not use it in a populated session due to the amount of network traffic it generates.


## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Force` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much force to apply to other RepulsionTreeItems within range. |
| `Radius` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The radius of influence this item has when interacting with other items. |

Fields
Collapse

## Behavior

## Examples

## See Also

[RepulsionTreeSimulator](https://wiki.resonite.com/Component:RepulsionTreeSimulator "Component:RepulsionTreeSimulator")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:RepulsionTreeItem&oldid=91448](https://wiki.resonite.com/index.php?title=Component:RepulsionTreeItem&oldid=91448)"

Contents