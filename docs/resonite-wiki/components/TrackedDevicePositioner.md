# Component:TrackedDevicePositioner

> Source: https://wiki.resonite.com/Component:TrackedDevicePositioner

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/5/52/TrackedDevicePositionerComponent.png/510px-TrackedDevicePositionerComponent.png)](https://wiki.resonite.com/File:TrackedDevicePositionerComponent.png) **Tracked Device Positioner** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **TrackedDevicePositioner** component is used to get information from the user's input system to get positioning data for tracked objects like headset, hands, and full body trackers.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `DeviceIndex` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The input Device by index to track. |
| `CorrespondingBodyNode` | **[BodyNode](https://wiki.resonite.com/Type:BodyNode "Type:BodyNode")** | The body node of the found input Device tracker. |
| `AutoBodyNode` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [BodyNode](https://wiki.resonite.com/Type:BodyNode "Type:BodyNode") >** | If present, use this to find the input Device to track rather than `DeviceIndex`. |
| `AlwaysRenderModel` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to always render the tracker Debug model regardless of if its mapped to a 3d model. |
| `ReferenceModel` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot of the debug model visual. |
| `BodyNodeRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | acts as an offset for the actual position of a Tracked object. |
| `ObjectSlot` | **[AvatarObjectSlot](https://wiki.resonite.com/Component:AvatarObjectSlot "Component:AvatarObjectSlot")** | The avatar object slot this component is driving. |
| `IsTracking` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the input Device is tracking or lost its tracking. |
| `IsActive` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the input Device is enabled. |
| `IsSimulated` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the device is being simulated instead by the locomotion animation system. |
| `CreateAvatarObjectSlot` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to create an avatar object slot component on a slot named "BodyNode" under this component slot if `BodyNodeRoot` is null. |
| `PoseFilter` | **[UserPoseController](https://wiki.resonite.com/Component:UserPoseController "Component:UserPoseController")** | The pose controller for this component to filter its position and movement based on if this component should be filtered. |

Fields
Collapse

## Usage

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Component:AvatarObjectSlot](https://wiki.resonite.com/Component:AvatarObjectSlot "Component:AvatarObjectSlot")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:TrackedDevicePositioner&oldid=106594](https://wiki.resonite.com/index.php?title=Component:TrackedDevicePositioner&oldid=106594)"

Contents