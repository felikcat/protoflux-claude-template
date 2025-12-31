# Component:MultiUserAvatarAnchor

> Source: https://wiki.resonite.com/Component:MultiUserAvatarAnchor

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:MultiUserAvatarAnchor&diff=94817) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/4/4e/MultiUserAvatarAnchorComponent.png/510px-MultiUserAvatarAnchorComponent.png)](https://wiki.resonite.com/File:MultiUserAvatarAnchorComponent.png) **MultiUserAvatarAnchor** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

Multi User Avatar anchor allows you to auto generate anchors, but only if you have a [collider](https://wiki.resonite.com/Collider "Collider") on the same slot as the multi anchor. It uses an [IAvatarAnchor type](https://wiki.resonite.com/Type:IAvatarAnchor "Type:IAvatarAnchor") component as a template, and generates them in a shape based on a Snapper ( [Snap Circle Component](https://wiki.resonite.com/Component:SnapCircle "Component:SnapCircle") or [Snap Sphere Component](https://wiki.resonite.com/Component:SnapSphere "Component:SnapSphere") to name a couple).

The snapper component determines how the users will be positioned when clicking on the object. If the anchor then anchors the user, and the user position is further determined by the anchor's positioning settings. If the anchor position in global space is too close to another anchor (determined by field MinDistance), then the user will not be anchored.

This component doesn't fall under a [IAvatarAnchor type](https://wiki.resonite.com/Type:IAvatarAnchor "Type:IAvatarAnchor"), and as such cannot be referenced by ProtoFlux. This means you can only anchor users with this component if they explicitly click on the anchor.

It also doesn't give confirmation for clicking actions, which may be a bug.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `AnchorPointSnap` | **[IPointSnappable](https://wiki.resonite.com/index.php?title=Type:IPointSnappable&action=edit&redlink=1 "Type:IPointSnappable (page does not exist)")** | A Snappable from [snapping category](https://wiki.resonite.com/Category:Components:Transform:Snapping "Category:Components:Transform:Snapping") |
| `MaxUsers` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | the maximum users that can be in this multi anchor |
| `MinDistance` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How close a new anchor can be to another when a user clicks on the anchor before it denies it. The location of the anchor before this check is done is determined by the component in AnchorPointSnap. |
| `Template` | **[IAvatarAnchor](https://wiki.resonite.com/Type:IAvatarAnchor "Type:IAvatarAnchor")** | The [IAvatarAnchor](https://wiki.resonite.com/Type:IAvatarAnchor "Type:IAvatarAnchor") to use as a template for making anchors. will duplicate the slot the anchor is on that this is referencing |
| `AnchorsRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | what shape to put the anchors when they are generated. The part of the shape the anchor is placed on is determined by the point the user clicked on. If user clicks on left side of a cube, user is positioned on the left face. |
| `AcceptOutOfSightTouch` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether or not to allow interaction with this component if it is out of the user's view. |
| `AcceptPhysicalTouch` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to allow [Component:TipTouchSources](https://wiki.resonite.com/Component:TipTouchSource "Component:TipTouchSource") to interact with/activate this component. |
| `AcceptRemoteTouch` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this component allows interaction via the user's interaction laser. |

Fields
Collapse

## Usage

## Examples

## See Also

[Snapping components](https://wiki.resonite.com/Category:Components:Transform:Snapping "Category:Components:Transform:Snapping")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:MultiUserAvatarAnchor&oldid=94817](https://wiki.resonite.com/index.php?title=Component:MultiUserAvatarAnchor&oldid=94817)"

Contents