# Component:AvatarFacetAnchor

> Source: https://wiki.resonite.com/Component:AvatarFacetAnchor

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/b/b8/AvatarFacetAnchorComponent.png/510px-AvatarFacetAnchorComponent.png)](https://wiki.resonite.com/File:AvatarFacetAnchorComponent.png) **Avatar Facet Anchor** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

Avatar Facet Anchor is a component that is used to position a userspace facet anchor to the slot this is on.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `FacetAnchorPoint` | **[FacetAnchorPoint](https://wiki.resonite.com/Type:FacetAnchorPoint "Type:FacetAnchorPoint")** | Which facet anchor should be positioned at the slot this component is on. |
| `OverrideState` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >** | Whether to force this anchor to stay on or off. |

Fields
Collapse

## Usage

Will not work if the component's active user is not the local user.

## Examples

Is usually auto generated on an avatar's hands, head, and arms so that facet anchors know where to position themselves.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AvatarFacetAnchor&oldid=93776](https://wiki.resonite.com/index.php?title=Component:AvatarFacetAnchor&oldid=93776)"

Contents