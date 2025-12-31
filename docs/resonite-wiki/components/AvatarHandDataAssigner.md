# Component:AvatarHandDataAssigner

> Source: https://wiki.resonite.com/Component:AvatarHandDataAssigner

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:AvatarHandDataAssigner&diff=94875) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/1/11/AvatarHandDataAssignerComponent.png/510px-AvatarHandDataAssignerComponent.png)](https://wiki.resonite.com/File:AvatarHandDataAssignerComponent.png) **AvatarHandDataAssigner** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **AvatarHandDataAssigner** component is usually located on avatar hands, and is used to assign key objects that make a hand work like tip touch sources and the avatar object controlling it.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `TargetReference` | **[SyncRef\`1](https://wiki.resonite.com/Type:SyncRef%601 "Type:SyncRef`1") < [IFingerPoseSourceComponent](https://wiki.resonite.com/Type:IFingerPoseSourceComponent "Type:IFingerPoseSourceComponent") >** | A field to assign a finger pose source to when the avatar above this component is equipped. Usually the `PoseSource` on a [Component:HandPoser](https://wiki.resonite.com/Component:HandPoser "Component:HandPoser") is specified here. |
| `TouchSource` | **[TipTouchSource](https://wiki.resonite.com/Component:TipTouchSource "Component:TipTouchSource")** | A tip touch source component to put data into when the avatar above this component is equipped. |
| `VibrationRelay` | **[VibrationDeviceRelay](https://wiki.resonite.com/Component:VibrationDeviceRelay "Component:VibrationDeviceRelay")** | A vibration device relay component to put data into when the avatar above this component is equipped. |
| `Chirality` | **[Chirality](https://wiki.resonite.com/Type:Chirality "Type:Chirality")** | Whether this component should assign data from the left or right hand data sets. |
| `_equippingSlot` | **[AvatarObjectSlot](https://wiki.resonite.com/Component:AvatarObjectSlot "Component:AvatarObjectSlot")** | This field is auto filled with the avatar object slot that is controlling the tip touch source and other components specified by this component. |

Fields
Collapse

## Usage

This component needs to be under an avatar in order to work, and is used to manage avatar hands.

## Examples

## See Also

- [Component:HandPoser](https://wiki.resonite.com/Component:HandPoser "Component:HandPoser")
- [Finger Posing System](https://wiki.resonite.com/Finger_Posing_System "Finger Posing System")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AvatarHandDataAssigner&oldid=94875](https://wiki.resonite.com/index.php?title=Component:AvatarHandDataAssigner&oldid=94875)"

Contents