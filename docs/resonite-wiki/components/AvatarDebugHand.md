# Component:AvatarDebugHand

> Source: https://wiki.resonite.com/Component:AvatarDebugHand

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:AvatarDebugHand&diff=96395) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/1/1f/AvatarDebugHandComponent.png/510px-AvatarDebugHandComponent.png)](https://wiki.resonite.com/File:AvatarDebugHandComponent.png) **AvatarDebugHand** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

Debug hand is a component that is used to show a debug visual when the [Biped Rig Component](https://wiki.resonite.com/Component:BipedRig "Component:BipedRig") has its "Debug Hand" [sync delegate](https://wiki.resonite.com/Sync_Delegate "Sync Delegate") pressed.

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This game element is a debug item. Elements like this may be removed at any time without warning, and creations should not rely on it.


## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `_objects` | _[list](https://wiki.resonite.com/Type:SyncRefList%601 "Type:SyncRefList`1")_ of **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slots of the mesh renderers that are being used to debug the hand. |
| `_materialTarget` | **[HierarchyMaterialTarget](https://wiki.resonite.com/Component:HierarchyMaterialTarget "Component:HierarchyMaterialTarget")** | The component used as a reference to apply `_material` to the debug when `_material` changes. |
| `_material` | **[PBS\_Metallic](https://wiki.resonite.com/PBS_Metallic "PBS Metallic")** | The material this component is using to render the visual |

Fields
Collapse

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AvatarDebugHand&oldid=96395](https://wiki.resonite.com/index.php?title=Component:AvatarDebugHand&oldid=96395)"

Contents