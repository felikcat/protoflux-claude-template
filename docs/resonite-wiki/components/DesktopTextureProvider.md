# Component:DesktopTextureProvider

> Source: https://wiki.resonite.com/Component:DesktopTextureProvider

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:DesktopTextureProvider&diff=92322) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/f/f4/DesktopTextureProviderComponent.png/510px-DesktopTextureProviderComponent.png)](https://wiki.resonite.com/File:DesktopTextureProviderComponent.png) **Desktop Texture Provider** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **DesktopTextureProvider** component only works in user space. This component is an [ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D") and can be used as a texture. This texture is able to display what is on any particular monitor on a user's machine. This component is commonly used in the desktop tab on a user's [Dash](https://wiki.resonite.com/Dash "Dash").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `DisplayIndex` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | What monitor to get image data for. |

Fields
Collapse

## Usage

This should not be used by the user, but it could be used to make a special facet. Insert the component into a texture field on a material to display it.

## Examples

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:DesktopTextureProvider&oldid=92322](https://wiki.resonite.com/index.php?title=Component:DesktopTextureProvider&oldid=92322)"

Contents