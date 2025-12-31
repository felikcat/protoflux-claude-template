# Component:HierarchyMaterialTarget

> Source: https://wiki.resonite.com/Component:HierarchyMaterialTarget

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:HierarchyMaterialTarget&diff=98523) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/e/e7/HierarchyMaterialTargetComponent.png/510px-HierarchyMaterialTargetComponent.png)](https://wiki.resonite.com/File:HierarchyMaterialTargetComponent.png) **Hierarchy Material Target** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **HierarchyMaterialTarget** component signals that a [slot](https://wiki.resonite.com/Slot "Slot") [tagged](https://wiki.resonite.com/Tag "Tag") with this component you are hitting with the [Material Tool](https://wiki.resonite.com/Material_Tool "Material Tool") is an appropriate target to look for materials in.

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

If this component is applied to the root of an avatar, when a material is applied to the avatar it will look for any mesh renderers in the hierarchy and apply the material.

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:HierarchyMaterialTarget&oldid=98523](https://wiki.resonite.com/index.php?title=Component:HierarchyMaterialTarget&oldid=98523)"

Contents