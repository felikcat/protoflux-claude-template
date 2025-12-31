# Component:ReflectionProbeSH2

> Source: https://wiki.resonite.com/Component:ReflectionProbeSH2

Collapse **Component image**

[File:ReflectionProbeSH2Component.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=ReflectionProbeSH2Component.png "File:ReflectionProbeSH2Component.png") **Reflection Probe SH2** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Reflection Probe SH2** component is used to turn what a [ReflectionProbe](https://wiki.resonite.com/Component:ReflectionProbe "Component:ReflectionProbe") sees into a spherical harmonic for use in ambient lighting like a [AmbientLightSH2](https://wiki.resonite.com/Component:AmbientLightSH2 "Component:AmbientLightSH2") component.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Probe` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [ReflectionProbe](https://wiki.resonite.com/Component:ReflectionProbe "Component:ReflectionProbe") >** | The probe to get color data from. |
| `AmbientLight` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[SphericalHarmonicsL2\`1](https://wiki.resonite.com/Type:SphericalHarmonicsL2%601 "Type:SphericalHarmonicsL2`1") < [ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX") >** | `Probe`'s sampled data as SH2 color data for ambient lighting usage. |
| `Order0Scale` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The scale factor for Order 0 for the spherical harmonics. |
| `Order1Scale` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The scale factor for Order 1 for the spherical harmonics. |
| `Order2Scale` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The scale factor for Order 2 for the spherical harmonics. |

Fields
Collapse

## Usage

Can be used to drive a [AmbientLightSH2](https://wiki.resonite.com/Component:AmbientLightSH2 "Component:AmbientLightSH2") component via a value copy or by drag and dropping this component's `AmbientLight` into that component's value

## Examples

## See Also

- [Component:AmbientLightSH2](https://wiki.resonite.com/Component:AmbientLightSH2 "Component:AmbientLightSH2")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ReflectionProbeSH2&oldid=106538](https://wiki.resonite.com/index.php?title=Component:ReflectionProbeSH2&oldid=106538)"

Contents