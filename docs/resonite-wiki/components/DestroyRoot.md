# Component:DestroyRoot

> Source: https://wiki.resonite.com/Component:DestroyRoot

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:DestroyRoot&diff=98515) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/5/55/DestroyRootComponent.png/510px-DestroyRootComponent.png)](https://wiki.resonite.com/File:DestroyRootComponent.png) **Destroy Root** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Destroy Root** component marks the [slot](https://wiki.resonite.com/Slot "Slot") [tagged](https://wiki.resonite.com/Tag "Tag") with the component where an object's root is for destroying grabbed objects if the game cannot find an object root component above the grabbed object.

Keep in mind, the grabber checks for object roots and destroy roots **after** releasing the object, which depending on the object and it's position will put it back where it was before it was grabbed. meaning this component can destroy the root object if a sub grabbed object is destroyed.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |

Fields
Collapse

## Usage

## Examples

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:DestroyRoot&oldid=98515](https://wiki.resonite.com/index.php?title=Component:DestroyRoot&oldid=98515)"

Contents