# Component:CameraPortal

> Source: https://wiki.resonite.com/Component:CameraPortal

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/1/12/CameraPortalComponent.png/510px-CameraPortalComponent.png)](https://wiki.resonite.com/File:CameraPortalComponent.png) **Camera Portal** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

Camera Portal, Also known as: Mirror, Portal, Gateway, Non Euclidean, and Bigger on the inside thing. This component allows for making a flat surface appear to have something on the other side.

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Renderer` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [MeshRenderer](https://wiki.resonite.com/Component:MeshRenderer "Component:MeshRenderer") >** | The renderer that the geometry is being used for the effect. This really only works best with flat surfaces, so use a quad in the target mesh renderer. |
| `ReflectionTexture` | **[RenderTexture](https://wiki.resonite.com/Type:RenderTexture "Type:RenderTexture")** | The render texture that this component should render what it wants to display to. This texture only works with a [Reflection Material](https://wiki.resonite.com/Component:ReflectionMaterial "Component:ReflectionMaterial") that goes on the `Render`'s mesh. |
| `PlaneOffset` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How far away from the surface the mirror or portal should render from. This doesn't need to be touched for a mirror, and causes some weird effects. |
| `PlaneNormal` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | Rotates what the mirror is rendering. this can can cause some very strange effects for Mirrors and Portals, and is best understood by playing with it. |
| `RenderMode` | **[CameraPortal.Mode](https://wiki.resonite.com/Component:CameraPortal#Mode)** | Whether this CameraPortal should act as a Mirror (Silver mirror) or as a Portal (Gateway, Non Euclidean, Tardis, ETC) |
| `PortalTarget` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot that should be used as a position to render from. When using Mirror `RenderMode`, keep this as the same slot as `Renderer`. When using Portal `RenderMode`, set the slot as the thing you're trying to make a gateway to visually (for a tardis, this would be the interior entrance somewhere else in the world) |
| `OverrideClear` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [CameraClearMode](https://wiki.resonite.com/Type:CameraClearMode "Type:CameraClearMode") >** | The type of color to clear when rendering. Functionally identical to the OverrideClear on a [Camera](https://wiki.resonite.com/Component:Camera "Component:Camera") |
| `ClearColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | If using "Color" for `OverrideClear` use this color. |
| `DisablePerPixelLights` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Disables lighting from points or spots in the projected image, which helps performance. |
| `DisableShadows` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Disable lights casting shadows in the projected image, which helps performance. |
| `OverrideFarClip` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | Override the default farclip from 4096 to this value when enabled. |
| `OverrideNearClip` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | Override the default nearclip from ~0 to this value when enabled. |

Fields
Collapse

## Mode

| Name | Value | Description |
| --- | --- | --- |
| `Mirror` | 0 | Essentially makes the camera portal act as a Silver mirror. |
| `Portal` | 1 | Essentially makes the camera portal act as a Gateway, Non Euclidean effect, Tardis door like effect. |

Values

## Behavior

This component does not allow for recursion (So you cannot put two mirrors in front and behind and expect them to reflect each other, or portal each other).

Currently, this component does not support culling of objects via object layers, and captures everything the local user currently can render via their POV. there is no way of changing this at the current moment.

## Examples

This component is used in mirrors to make what is behind you appear to be on the other side like a mirror, and it is also useful for portals or making a T.A.R.D.I.S.

## See Also

[Camera](https://wiki.resonite.com/Component:Camera "Component:Camera")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:CameraPortal&oldid=100802](https://wiki.resonite.com/index.php?title=Component:CameraPortal&oldid=100802)"

Contents