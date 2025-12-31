# Component:VirtualParent

> Source: https://wiki.resonite.com/Component:VirtualParent

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:VirtualParent&diff=93827) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/4/4f/VirtualParentComponent.png/510px-VirtualParentComponent.png)](https://wiki.resonite.com/File:VirtualParentComponent.png) **VirtualParent** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

## Description

The Virtual Parent Component is used to make a [Slot](https://wiki.resonite.com/Slot "Slot") act as the child of another Slot without needing to be in the normal hierarchy order. This can be useful when you need it to respond in a certain way using transforms of the overriding parent.

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

The Virtual Parent Component will not automatically update the slot unless the overriding parent slot has moved, rotated, or scaled (or in some way updated its current transform)


The different ways to force this Slot (that has the Virtual Parent Component on it) to update its own transform, is to move it by grabbing it, using other components to move it, or using Flux.

You can use the provided local offset fields to then further position this slot from its virtual parent.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `OverrideParent` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | If not null, the slot that the object gets reparented to |
| `_targetPos` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | Position to be driven by parent's position. |
| `_targetRot` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | Rotation to be driven by parent's rotation. |
| `_targetScl` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | Scale to be driven by parent's scale. |
| `LocalPosition` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | Object's position relative to parent. |
| `LocalRotation` | **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | Object's rotation relative to parent. |
| `LocalScale` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | Object's scale relative to parent. |

Fields
Collapse

## Usage

## Examples

## See Also

- [Component:CopyGlobalTransform](https://wiki.resonite.com/Component:CopyGlobalTransform "Component:CopyGlobalTransform")
- [Component:CopyGlobalScale](https://wiki.resonite.com/Component:CopyGlobalScale "Component:CopyGlobalScale")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:VirtualParent&oldid=93827](https://wiki.resonite.com/index.php?title=Component:VirtualParent&oldid=93827)"

Contents