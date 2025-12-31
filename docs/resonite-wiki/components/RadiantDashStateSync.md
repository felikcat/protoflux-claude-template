# Component:RadiantDashStateSync

> Source: https://wiki.resonite.com/Component:RadiantDashStateSync

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/c/c2/RadiantDashStateSyncComponent.png/510px-RadiantDashStateSyncComponent.png)](https://wiki.resonite.com/File:RadiantDashStateSyncComponent.png) **RadiantDashStateSync** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **RadiantDashStateSync** component is a [userspace](https://wiki.resonite.com/Userspace "Userspace") component that grabs the current [dash component](https://wiki.resonite.com/Component:RadiantDash "Component:RadiantDash") in the userspace world and cross synchronizes its values with the dash.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `IsFreeform` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the userspace dash is set to freeform movement. |
| `IsOpen` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the userspace dash is currently open. |
| `Curvature` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | What the curvature of the dash is currently. |

Fields
Collapse

## Usage

Best used when attached to an item that will exist on the dash, like a facet.

## Examples

Can be used to get user settings for a dash within a facet.

## See Also

- [Dash](https://wiki.resonite.com/Dash "Dash")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:RadiantDashStateSync&oldid=99740](https://wiki.resonite.com/index.php?title=Component:RadiantDashStateSync&oldid=99740)"

Contents