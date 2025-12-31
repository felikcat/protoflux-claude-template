# Component:LocomotionPermissions

> Source: https://wiki.resonite.com/Component:LocomotionPermissions

## Introduction

The LocomotionPermissions component allows you to control what locomotions users can use in your world.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `LocomotionListMode` | **[ListFilterMode](https://wiki.resonite.com/Type:ListFilterMode "Type:ListFilterMode")** | Whether to blacklist or whitelist the `Locomotions`. |
| `Locomotions` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[LocomotionPermissions.LocomotionFilter](https://wiki.resonite.com/Component:LocomotionPermissions#LocomotionFilter)** | List of `Locomotions` to blacklist/whitelist. |
| `Scaling` | **[PermissionState](https://wiki.resonite.com/Type:PermissionState "Type:PermissionState")** | Whether self scale is Disallowed, Allowed, or [Edit Mode](https://wiki.resonite.com/Edit_Mode "Edit Mode") Only. |
| `MinScale` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Minimum scale |
| `MaxScale` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Maximum scale |
| `JumpToUser` | **[PermissionState](https://wiki.resonite.com/Type:PermissionState "Type:PermissionState")** | Whether jumping to users is Disallowed, Allowed, or [Edit Mode](https://wiki.resonite.com/Edit_Mode "Edit Mode") Only. |

Fields
Collapse

## Usage

### Find Roles slot

You will need to first find the **Roles** slot, typically it is directly under the world's [Root](https://wiki.resonite.com/Root "Root"). Under the Roles slot there is a list of the roles you can select from.

### Find/attach the permission component

You will need to find the LocomotionPermissions component on the selected role slot, if the component is not there you can attach one with the component browser from the **Permissions** component folder.

### Configuration

[![](https://wiki.resonite.com/images/thumb/e/e9/Locomotion_blacklist.webp/300px-Locomotion_blacklist.webp.png)](https://wiki.resonite.com/File:Locomotion_blacklist.webp) A locomotion blacklist

The LocomotionPermissions component can be switched between Blacklisting and Whitelisting the locomotions supplied in the Locomotions list. Valid LocomotionTypes you can enter are:

- FrooxEngine.NoclipLocomotion
- FrooxEngine.PhysicalLocomotion
- FrooxEngine.TeleportLocomotion
- FrooxEngine.GrabWorldLocomotion
- FrooxEngine.SlideLocomotion

Next you will need to select what roles the component effects.

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:LocomotionPermissions&oldid=97607](https://wiki.resonite.com/index.php?title=Component:LocomotionPermissions&oldid=97607)"

Contents