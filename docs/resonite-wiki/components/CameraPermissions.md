# Component:CameraPermissions

> Source: https://wiki.resonite.com/Component:CameraPermissions

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:CameraPermissions&diff=91198) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/e/e8/CameraPermissionsComponent.png/510px-CameraPermissionsComponent.png)](https://wiki.resonite.com/File:CameraPermissionsComponent.png) **Camera Permissions** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The Camera Permissions component allows you to set up who can use certain camera modes on the streaming camera. Currently, the component allows setting permissions for camera modes per role.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `CameraModeFilterMode` | **[ListFilterMode](https://wiki.resonite.com/Type:ListFilterMode "Type:ListFilterMode")** | Whether to allow or disallow the `CameraModes` |
| `CameraModes` | _direct_ **[SyncFieldList\`1](https://wiki.resonite.com/Type:SyncFieldList%601 "Type:SyncFieldList`1") < [CameraPositioningMode](https://wiki.resonite.com/Type:CameraPositioningMode "Type:CameraPositioningMode") >** | List of Camera modes which decide how a stream camera can look at users and/or the world. |
| `AllowFramingOtherUsers` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether focusing the camera on other user is allowed. |

Fields
Collapse

## Usage

First, add an item to the list of camera modes, and select a role at the bottom. Then, use `CameraModeFilterMode` to determine if users can use any of the items in the list of camera modes.

## Examples

If the `CameraModeFilterMode` field is set to `Whitelist` and `Group` is added to the `CameraMode` list, then the selected role can only use the `Group` mode with their stream cameras.

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:CameraPermissions&oldid=91198](https://wiki.resonite.com/index.php?title=Component:CameraPermissions&oldid=91198)"

Contents