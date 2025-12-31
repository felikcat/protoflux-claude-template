# Component:LightOrb

> Source: https://wiki.resonite.com/Component:LightOrb

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/d/d6/LightOrbComponent.png/510px-LightOrbComponent.png)](https://wiki.resonite.com/File:LightOrbComponent.png) **Light Orb** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Light Orb** component is used as a visual for lights created by the [Light Tool](https://wiki.resonite.com/Light_Tool "Light Tool").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `FlipOnTouch` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this can be toggled by touching a collider on the same slot. |
| `Light` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [Light](https://wiki.resonite.com/Component:Light "Component:Light") >** | The light to control. |
| `EmissionColor` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The field to drive to control the emission color of the light. |
| `AcceptPhysicalTouch` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to allow [Component:TipTouchSources](https://wiki.resonite.com/Component:TipTouchSource "Component:TipTouchSource") to interact with/activate this component. |
| `AcceptRemoteTouch` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this component allows interaction via the user's interaction laser. |

Fields
Collapse

## Usage

Not used directly by the user.

## Examples

- created by the [Light Tool](https://wiki.resonite.com/Light_Tool "Light Tool").

## See Also

- [Light Tool](https://wiki.resonite.com/Light_Tool "Light Tool")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:LightOrb&oldid=103808](https://wiki.resonite.com/index.php?title=Component:LightOrb&oldid=103808)"

Contents