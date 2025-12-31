# Component:AvatarRenderSettings

> Source: https://wiki.resonite.com/Component:AvatarRenderSettings

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:AvatarRenderSettings&diff=93404) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/0/0c/AvatarRenderSettingsComponent.png/510px-AvatarRenderSettingsComponent.png)](https://wiki.resonite.com/File:AvatarRenderSettingsComponent.png) **AvatarRenderSettings** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

Avatar Render Settings is a component that can be placed anywhere on an avatar for it to work. This component changes the internal camera settings for the first person view for a user wearing an avatar with this component under it by optionally changing the far and/or near clip values of the POV camera.

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `NearClip` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | If not null, changes the NearClip of the user's POV camera when this component is under the user's avatar hierarchy. |
| `FarClip` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | If not null, changes the FarClip of the user's POV camera when this component is under the user's avatar hierarchy. |

Fields
Collapse

## Behavior

This component does not start working on an avatar when added, until the avatar is re-equipped. After this, changing values on the component change what the user sees live. This component can be used to extend the distance a user can see, which by default is 4096 meters multipled by user global scale.

## Examples

Can be used to prevent a user from seeing the snout of an avatar, or the hair on an avatars face. This can also be used to allow a user to be able to see objects outside of normal clipping distance by making `FarClip` larger than 4096.

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AvatarRenderSettings&oldid=93404](https://wiki.resonite.com/index.php?title=Component:AvatarRenderSettings&oldid=93404)"

Contents