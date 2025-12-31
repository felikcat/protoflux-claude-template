# Component:GrabbableReceiverSurface

> Source: https://wiki.resonite.com/Component:GrabbableReceiverSurface

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:GrabbableReceiverSurface&diff=95641) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/e/e0/GrabbableReceiverSurfaceComponent.png/510px-GrabbableReceiverSurfaceComponent.png)](https://wiki.resonite.com/File:GrabbableReceiverSurfaceComponent.png) **GrabbableReceiverSurface** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **GrabbableReceiverSurface** component allows you to set up an object so that [Grabbable](https://wiki.resonite.com/Component:Grabbable "Component:Grabbable") objects snap to its surface when a user releases the [Grabbable](https://wiki.resonite.com/Component:Grabbable "Component:Grabbable") object within range of it. For a volume based alternative, see [Grabbable Parenter](https://wiki.resonite.com/Component:GrabbableParenter "Component:GrabbableParenter").

Add Component Path: Transform > Interaction > GrabbableReceiverSurface.

# Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `ParentPlaced` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the [Grabbable](https://wiki.resonite.com/Component:Grabbable "Component:Grabbable") object gets reparented to this object's Slot or the Slot specified in OverrideParent. |
| `OverrideParent` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | If not null, the slot that the [Grabbable](https://wiki.resonite.com/Component:Grabbable "Component:Grabbable") object gets reparented to, if ParentPlaced is true. |
| `TweenTime` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The amount of time in seconds for the animation effect when the object snaps to the surface. |
| `MaxDistance` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How far away in meters something released gets grabbed. |
| `Offset` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The distance from the surface that the [Grabbable](https://wiki.resonite.com/Component:Grabbable "Component:Grabbable") object will stop at. |
| `CheckOffset` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How far away from the surface that the object ignores before it starts looking for released objects. |
| `Directions` | _direct_ **[SyncFieldList\`1](https://wiki.resonite.com/Type:SyncFieldList%601 "Type:SyncFieldList`1") < [Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3") >** | List of directions a [Grabbable](https://wiki.resonite.com/Component:Grabbable "Component:Grabbable") object can be received from. |
| `TagFilter` | _direct_ **[TagFilter](https://wiki.resonite.com/Type:TagFilter "Type:TagFilter")** | A filter that limits what can be picked up by this surface. |

Fields
Collapse

# Behavior

When a GrabbableReceiverSurface is setup on an object, it will become visible to Grabbable objects when they are released from a user's grab. When this occurs the Surface will carry out some checks and if these pass the object will snap to the GrabbableReceiverSurface. If the `ParentPlaced` checkbox is enable the Grabbable will be parented to the surface or the slot specified in `OverrideParent`

## Explanation of the Checks

These are a little complicated but if you want to fully understand what happens it is provided.

When a user is holding a Grabbable object and lets go (releases it):

1. The Grabbable object will look around it in its vicinity using a sphere collider based on the Object's bounding box plus a radius defined on the User's Hand. The hand radius is defined by a sphere made from a Bounding box of all the released objects.
2. If this collider overlaps with any objects which have GrabbableRecieverSurface attached to them then the Grabbable will perform some checks on each surface.
3. First it asks the Surface to check its distance from the Grabbable object.
1. The distance check first calculates if a Raycast from the released object towards the surface would hit in the directions specified in the component.
2. If the Raycast would hit a distance is then calculated.
3. This distance varies depending on the directions specified in the component's properties.
      - For example, placing an object on top of a cube from above has a shorter distance to the top of the Cube than the bottom of a cube because the distance from above the cube to the bottom face of the cube is greater.
4. If this distance is to great as specified in the component's properties a second check using the released object's bounding box corners is also computed
5. After both distance checks a final distance value is provided.
6. The [Grabbable](https://wiki.resonite.com/Component:Grabbable "Component:Grabbable") then selects the surface with the smallest distance and tells the Surface to receive it.
7. The Surface will then position the [Grabbable](https://wiki.resonite.com/Component:Grabbable "Component:Grabbable") upon the surface using an Animation of a `Tween Time` value is set.
8. The Surface will then parent the [Grabbable](https://wiki.resonite.com/Component:Grabbable "Component:Grabbable") to itself or the `OverrideParent` location if the `ParentPlaced` checkbox is checked.

# Examples

[ProbablePrime](https://wiki.resonite.com/User:ProbablePrime "User:ProbablePrime")'s tutorial on GrabbleReceiverSurface:

![](https://i.ytimg.com/vi/9IZI3ui-RLY/hqdefault.jpg)

[OLD: Neos VR Tutorial: GrabbableReceiverSurface for Easy Shelves and Tables](https://www.youtube-nocookie.com/embed/9IZI3ui-RLY?autoplay=1)

Load video

YouTube

YouTube might collect personal data. [Privacy Policy](https://www.youtube.com/howyoutubeworks/user-settings/privacy/)

ContinueDismiss

# Frequently Asked Questions

## Can objects which are not grabbed be received?

No, this component only works with [Grabbable](https://wiki.resonite.com/Component:Grabbable "Component:Grabbable") objects which are released by a user.

## Can this be used with objects that are not Grabbable?

No, It cannot be used with objects that do not have a [Grabbable](https://wiki.resonite.com/Component:Grabbable "Component:Grabbable") component.

# See Also

- [Grabbable](https://wiki.resonite.com/Component:Grabbable "Component:Grabbable") for what this receives.
- [Grabbable Parenter](https://wiki.resonite.com/Component:GrabbableParenter "Component:GrabbableParenter") For a volume alternative

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:GrabbableReceiverSurface&oldid=95641](https://wiki.resonite.com/index.php?title=Component:GrabbableReceiverSurface&oldid=95641)"

Contents