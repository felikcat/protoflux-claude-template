# Component:AvatarPoseFilterInstaller

> Source: https://wiki.resonite.com/Component:AvatarPoseFilterInstaller

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:AvatarPoseFilterInstaller&diff=93904) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/0/0c/AvatarPoseFilterInstallerComponent.png/510px-AvatarPoseFilterInstallerComponent.png)](https://wiki.resonite.com/File:AvatarPoseFilterInstallerComponent.png) **Avatar Pose Filter Installer** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **AvatarPoseFilterInstaller** component can be placed into slots below or on the same Slot as a Proxy on an avatar in order to auto install a pose filter on those parts upon equipping the avatar.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Filter` | **[IAvatarPoseFilter](https://wiki.resonite.com/Type:IAvatarPoseFilter "Type:IAvatarPoseFilter")** | the Pose Filter to install on an Avatar's pose node like the head, hands, arms, or feet. |
| `Priority` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | If this installer should run before other [IAvatarObjectComponents](https://wiki.resonite.com/index.php?title=Type:IAvatarObjectComponent&action=edit&redlink=1 "Type:IAvatarObjectComponent (page does not exist)"). |

Fields
Collapse

## Usage

Used to make an avatar with slow hands, or an avatar that has restricted movement with its limbs.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AvatarPoseFilterInstaller&oldid=93904](https://wiki.resonite.com/index.php?title=Component:AvatarPoseFilterInstaller&oldid=93904)"

Contents