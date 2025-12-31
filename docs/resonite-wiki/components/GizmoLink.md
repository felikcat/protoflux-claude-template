# Component:GizmoLink

> Source: https://wiki.resonite.com/Component:GizmoLink

Collapse **Component image**

[File:GizmoLinkComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=GizmoLinkComponent.png "File:GizmoLinkComponent.png") **Gizmo Link** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **GizmoLink** component handles the Interaction and connection of every [Gizmo](https://wiki.resonite.com/Gizmo "Gizmo") with their respective target. This is usually invisible to users and their inspectors, but upon opening a new inspector on a target of a Gizmo it appears. It is unknown if this is a bug. This component along with Gizmos do not save with items but Gizmos can save with a world.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `_worker` | **[Worker](https://wiki.resonite.com/index.php?title=Type:Worker&action=edit&redlink=1 "Type:Worker (page does not exist)")** | The logic handling this component. |
| `_gizmo` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [IComponentGizmo](https://wiki.resonite.com/Type:IComponentGizmo "Type:IComponentGizmo") >** | The Gizmo this is making a Link for. |
| `_type` | _direct_ **[SyncType](https://wiki.resonite.com/Type:SyncType "Type:SyncType")** | The C# Type of what this is targeting. |

Fields
Collapse

## Usage

Not used directly by the user.

## Examples

Attached automatically to slots that are targets of any [IComponentGizmo](https://wiki.resonite.com/Type:IComponentGizmo "Type:IComponentGizmo").

## See Also

- [Gizmo](https://wiki.resonite.com/Gizmo "Gizmo")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:GizmoLink&oldid=96749](https://wiki.resonite.com/index.php?title=Component:GizmoLink&oldid=96749)"

Contents