# Component:Float4Driver

> Source: https://wiki.resonite.com/Component:Float4Driver

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:Float4Driver&diff=91330) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/5/52/Float4DriverComponent.png/510px-Float4DriverComponent.png)](https://wiki.resonite.com/File:Float4DriverComponent.png) **Float 4Driver** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The Float4Driver component can be used to drive a foat4 value, based on an X, Y, Z and a W value.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `X` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [Sync\`1](https://wiki.resonite.com/Type:Sync%601 "Type:Sync`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >>** | The field that holds the X value for the float4. If null, the X component of the float4 will be 0. |
| `Y` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [Sync\`1](https://wiki.resonite.com/Type:Sync%601 "Type:Sync`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >>** | The field that holds the Y value for the float4. If null, the Y component of the float4 will be 0. |
| `Z` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [Sync\`1](https://wiki.resonite.com/Type:Sync%601 "Type:Sync`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >>** | The field that holds the Z value for the float4. If null, the Z component of the float4 will be 0. |
| `W` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [Sync\`1](https://wiki.resonite.com/Type:Sync%601 "Type:Sync`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >>** | The field that holds the W value for the float4. If null, the W component of the float4 will be 0. |
| `Target` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float4](https://wiki.resonite.com/Type:Float4 "Type:Float4")** | The field that is driven to the constructed float4. |

Fields
Collapse

## Usage

## Examples

## Related Issues

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:Float4Driver&oldid=91330](https://wiki.resonite.com/index.php?title=Component:Float4Driver&oldid=91330)"

Contents