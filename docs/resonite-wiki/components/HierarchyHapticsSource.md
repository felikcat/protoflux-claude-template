# Component:HierarchyHapticsSource

> Source: https://wiki.resonite.com/Component:HierarchyHapticsSource

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/2/25/HierarchyHapticsSourceComponent.png/510px-HierarchyHapticsSourceComponent.png)](https://wiki.resonite.com/File:HierarchyHapticsSourceComponent.png) **Hierarchy Haptics Source** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **HiearchyHapticsSource** component every `Interval` seconds triggers a relative intensity haptics signal (Additive) of `RelativeIntensity`.

This works as part of the game's robust [Haptics](https://wiki.resonite.com/Haptics "Haptics") system.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `TargetHierarchy` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The hiearchy of haptics to trigger. If targeting an arm slot on an avatar, triggers all haptics under the arm and hand. For a VR user this would get their controller. |
| `Interval` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The amount of seconds to wait per trigger. Fires automatically every this many seconds. |
| `RelativeIntensity` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The relative haptics intensity amount to send each trigger. |

Fields
Collapse

## Usage

Attach to a slot and provide a slot to `TargetHiearchy` that is under a user to trigger haptics on. Then provide some values to adjust to the desired effect.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:HierarchyHapticsSource&oldid=96133](https://wiki.resonite.com/index.php?title=Component:HierarchyHapticsSource&oldid=96133)"

Contents