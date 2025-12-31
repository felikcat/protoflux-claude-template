# Component:CopyTransformFromWorld

> Source: https://wiki.resonite.com/Component:CopyTransformFromWorld

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/3/3d/CopyTransformFromWorldComponent.png/510px-CopyTransformFromWorldComponent.png)](https://wiki.resonite.com/File:CopyTransformFromWorldComponent.png) **CopyTransformFromWorld** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **CopyTransformFromWorld** component is used by the game to copy transforms from other worlds. This is mainly used by [userspace](https://wiki.resonite.com/Userspace "Userspace") to copy transforms from objects like [world orbs](https://wiki.resonite.com/Component:WorldOrb "Component:WorldOrb") when the user highlights them.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `CopyPosition` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to copy Position. |
| `CopyRotation` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to copy Rotation. |
| `CopyScale` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to copy Scale. |

Fields
Collapse

## Usage

## Examples

## See Also

- [Component:WorldOrb](https://wiki.resonite.com/Component:WorldOrb "Component:WorldOrb")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:CopyTransformFromWorld&oldid=100121](https://wiki.resonite.com/index.php?title=Component:CopyTransformFromWorld&oldid=100121)"

Contents