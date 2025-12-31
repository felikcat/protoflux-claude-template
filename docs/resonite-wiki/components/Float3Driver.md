# Component:Float3Driver

> Source: https://wiki.resonite.com/Component:Float3Driver

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:Float3Driver&diff=91329) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/0/09/Float3DriverComponent.png/510px-Float3DriverComponent.png)](https://wiki.resonite.com/File:Float3DriverComponent.png) **Float 3Driver** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The Float3Driver component can be used to drive a foat3 value, based on an X, Y and a Z value.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `X` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [Sync\`1](https://wiki.resonite.com/Type:Sync%601 "Type:Sync`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >>** | The field that holds the X value for the float3. If null, the X component of the float3 will be 0. |
| `Y` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [Sync\`1](https://wiki.resonite.com/Type:Sync%601 "Type:Sync`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >>** | The field that holds the Y value for the float3. If null, the Y component of the float3 will be 0. |
| `Z` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [Sync\`1](https://wiki.resonite.com/Type:Sync%601 "Type:Sync`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >>** | The field that holds the Z value for the float3. If null, the Z component of the float3 will be 0. |
| `Target` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field that is driven to the constructed float3. |

Fields
Collapse

## Usage

## Examples

## Related Issues

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:Float3Driver&oldid=91329](https://wiki.resonite.com/index.php?title=Component:Float3Driver&oldid=91329)"

Contents