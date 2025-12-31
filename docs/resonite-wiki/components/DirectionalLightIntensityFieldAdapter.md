# Component:DirectionalLightIntensityFieldAdapter

> Source: https://wiki.resonite.com/Component:DirectionalLightIntensityFieldAdapter

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/f/f7/DirectionalLightIntensityFieldAdapterComponent.png/510px-DirectionalLightIntensityFieldAdapterComponent.png)](https://wiki.resonite.com/File:DirectionalLightIntensityFieldAdapterComponent.png) **Directional Light Intensity Field Adapter** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **DirectionalLightIntensityFieldAdapter** component is used to convert intensity in a directional light from the old SRGB color space into linear when converting worlds.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Target` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The Float to drive with the converted value. |
| `Value` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The original value. |
| `Scale` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to multiply `Value` by. |

Fields
Collapse

## Usage

This is usually auto generated and not used by the user directly.

## Examples

Used to convert old content color into new content color for sun lights.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:DirectionalLightIntensityFieldAdapter&oldid=96453](https://wiki.resonite.com/index.php?title=Component:DirectionalLightIntensityFieldAdapter&oldid=96453)"

Contents