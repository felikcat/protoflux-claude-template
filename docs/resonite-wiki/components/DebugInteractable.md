# Component:DebugInteractable

> Source: https://wiki.resonite.com/Component:DebugInteractable

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/9/92/DebugInteractableComponent.png/510px-DebugInteractableComponent.png)](https://wiki.resonite.com/File:DebugInteractableComponent.png) **Debug Interactable** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **DebugInteractable** component is a [UIX](https://wiki.resonite.com/UIX "UIX") interactable that changes the color of an image on the same slot when the component area is interacted with.

This was possibly made by [Frooxius](https://wiki.resonite.com/User:Frooxius "User:Frooxius") while they were creating [UIX](https://wiki.resonite.com/UIX "UIX") during the UIX development of FrooxEngine.

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This game element is a debug item. Elements like this may be removed at any time without warning, and creations should not rely on it.


## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `TouchExitLock` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the component can have an exit event or not when touching the component is stopped. |
| `TouchEnterLock` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the component can have an enter event or not when touching the component is started. |

Fields
Collapse

## Usage

Attach to a slot of a UIX with an [Image component](https://wiki.resonite.com/Component:Image "Component:Image") to start debugging via touch.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Component:Image](https://wiki.resonite.com/Component:Image "Component:Image")
- [UIX](https://wiki.resonite.com/UIX "UIX")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:DebugInteractable&oldid=96380](https://wiki.resonite.com/index.php?title=Component:DebugInteractable&oldid=96380)"

Contents