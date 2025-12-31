# Component:Skybox

> Source: https://wiki.resonite.com/Component:Skybox

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/f/fb/SkyboxComponent.png/510px-SkyboxComponent.png)](https://wiki.resonite.com/File:SkyboxComponent.png) **Skybox** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

Can be used to specify the current material for the skybox and set the current skybox for the current world.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Material` | **[Material](https://wiki.resonite.com/Type:Material "Type:Material")** | The material to use for the skybox. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `SetActive:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Sets the current skybox for the world to this one. |

Triggers
Collapse

## Usage

Attach to a slot, put a [Component:Projection360Material](https://wiki.resonite.com/Component:Projection360Material "Component:Projection360Material") or a [Component:ProceduralSkyMaterial](https://wiki.resonite.com/Component:ProceduralSkyMaterial "Component:ProceduralSkyMaterial") in `Material` and hit the "Set Active Skybox" button to enable the skybox.

## Examples

In the root of the default world gridspace and any other Template.

## See Also

- [World](https://wiki.resonite.com/World "World")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:Skybox&oldid=99370](https://wiki.resonite.com/index.php?title=Component:Skybox&oldid=99370)"

Contents