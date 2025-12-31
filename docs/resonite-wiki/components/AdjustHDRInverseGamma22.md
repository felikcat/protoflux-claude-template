# Component:AdjustHDRInverseGamma22

> Source: https://wiki.resonite.com/Component:AdjustHDRInverseGamma22

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/e/e3/AdjustHDRInverseGamma22Component.png/510px-AdjustHDRInverseGamma22Component.png)](https://wiki.resonite.com/File:AdjustHDRInverseGamma22Component.png) **Adjust HDR Inverse Gamma 22** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

Drives a target field by applying a fixed inverse 2.2 HDR gamma from to an input value.

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Target` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The target field to drive the value of. |
| `Value` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The value to apply the gamma calculation to. |

Fields
Collapse

## Behavior

This node performs the same calculation as the [Apply HDR Inverse Gamma ColorX](https://wiki.resonite.com/ProtoFlux:Apply_HDR_Inverse_Gamma_ColorX "ProtoFlux:Apply HDR Inverse Gamma ColorX") ProtoFlux node, with a gamma value of 2.2.

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AdjustHDRInverseGamma22&oldid=91615](https://wiki.resonite.com/index.php?title=Component:AdjustHDRInverseGamma22&oldid=91615)"

Contents