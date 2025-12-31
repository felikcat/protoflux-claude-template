# Component:InteractionBlock

> Source: https://wiki.resonite.com/Component:InteractionBlock

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:InteractionBlock&diff=88782) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/5/53/InteractionBlockComponent.png/510px-InteractionBlockComponent.png)](https://wiki.resonite.com/File:InteractionBlockComponent.png) **InteractionBlock** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **InteractionBlock** component is used to block [UIX](https://wiki.resonite.com/UIX "UIX") interaction events from the [user](https://wiki.resonite.com/User "User"). It requires an [Image](https://wiki.resonite.com/Component:Image "Component:Image") on the same [Slot](https://wiki.resonite.com/Slot "Slot") this component is on for this to work.

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

Order matters, using the `OrderOffset` will determine what gets blocked based on the slot hierarchy. Keep in mind the layers of the slots, usually anything behind this component's slot (a lower `OrderOffset`) will no longer be interactable.


| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `TouchExitLock` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Blocks interactions when an interaction ends. |
| `TouchEnterLock` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Blocks interactions when an interaction starts. |

Fields
Collapse

## Usage

Any time you want to stop any UIX element from interacting (like having a popup menu to be on top of your main UIX), you can use this component to make the main UIX elements not respond to the user, making them focus on the newly spawned UIX.

## Examples

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:InteractionBlock&oldid=88782](https://wiki.resonite.com/index.php?title=Component:InteractionBlock&oldid=88782)"

Contents