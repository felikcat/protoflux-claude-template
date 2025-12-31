# Component:GrabToolSnapper

> Source: https://wiki.resonite.com/Component:GrabToolSnapper

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/d/df/GrabTooltipSnapperComponent.png/510px-GrabTooltipSnapperComponent.png)](https://wiki.resonite.com/File:GrabTooltipSnapperComponent.png) **Grab Tool Snapper** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **GrabToolSnapper** component snaps a grabbable component's slot on the same slot as this component to the tip of a tool or your tooltip anchor when the Grabbable is grabbed.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Offset` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | How far away from the tool the object should be upon grab. |

Fields
Collapse

## Usage

This component is mostly for internal use, it is what is responsible for the [ReferenceProxy](https://wiki.resonite.com/Component:ReferenceProxy "Component:ReferenceProxy") text that appears when you grab slots and fields in the inspector.

You can still use it if you would like, please check the behavior section.

# Behavior

If this component is added to a [IGrabbable](https://wiki.resonite.com/Type:IGrabbable "Type:IGrabbable") Object, when this object is grabbed it will be positioned at the tip of your Tool plus any offset specified in the offset field. On it's own this is not that usable but this is used internally with some UI Fields and Proxies to provide the blue text as shown above.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:GrabToolSnapper&oldid=94781](https://wiki.resonite.com/index.php?title=Component:GrabToolSnapper&oldid=94781)"

Contents