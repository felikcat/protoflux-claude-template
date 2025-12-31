# Component:GlowingSphereToggle

> Source: https://wiki.resonite.com/Component:GlowingSphereToggle

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/c/c9/GlowingSphereToggleComponent.png/510px-GlowingSphereToggleComponent.png)](https://wiki.resonite.com/File:GlowingSphereToggleComponent.png) **Glowing Sphere Toggle** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **GlowingSphereToggle** component can be used to toggle a boolean value when clicked.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `TargetField` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >** | The field to toggle. |
| `FadeSpeed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How fast to fade after being clicked. |
| `CooldownTime` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How long the user has to wait before they can toggle it again. |
| `Radius` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The size of the toggle sphere. |
| `GlowColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | What color the sphere should glow. |
| `_emissiveColor` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color to drive with the sphere color for emissive. |
| `_rimColor` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color to drive with the rim color. |
| `_sphereRadius` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The field to drive with the sphere radius. |
| `_sphereExtrude` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The field to drive with the sphere extrude value. |
| `_colliderRadius` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The field to drive with the collider radius. |

Fields
Collapse

## Usage

Attach to a slot and provide values as well as something to toggle for this component to work.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Component:ButtonToggle](https://wiki.resonite.com/Component:ButtonToggle "Component:ButtonToggle")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:GlowingSphereToggle&oldid=96762](https://wiki.resonite.com/index.php?title=Component:GlowingSphereToggle&oldid=96762)"

Contents