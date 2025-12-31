# Component:BooleanReferenceDriver

> Source: https://wiki.resonite.com/Component:BooleanReferenceDriver

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:BooleanReferenceDriver&diff=91235) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/0/03/BooleanReferenceDriver%601Component.png/510px-BooleanReferenceDriver%601Component.png)](https://wiki.resonite.com/File:BooleanReferenceDriver%601Component.png) **Boolean Reference Driver\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The BooleanReferenceDriver component is used to drive a reference to one value or another, depending on its State field.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `State` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether TargetReference should be driven to TrueTarget or to FalseTarget. |
| `TargetReference` | _direct_ **[RefDrive\`1](https://wiki.resonite.com/index.php?title=Type:RefDrive%601&action=edit&redlink=1 "Type:RefDrive`1 (page does not exist)") <T>** | The field that should be driven. |
| `FalseTarget` | **T** | The value that the field will be driven to if `State` is false. |
| `TrueTarget` | **T** | The value that the field will be driven to if `State` is true. |

Fields
Collapse

## Usage

Attach this component to a slot by first choosing what kind of value you want to boolean switch. See [Interface](https://wiki.resonite.com/Interface "Interface") on how similar types can be used that are different classes (Like materials for example). Once a type has been chosen, this component can be used to switch the value in a field between two different ones using `State`

## Examples

Can be used as an alternative to [Boolean Asset Driver](https://wiki.resonite.com/Component:BooleanAssetDriver "Component:BooleanAssetDriver") to switch assets, and as a way of switching slot references around

## Related Issues

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:BooleanReferenceDriver&oldid=91235](https://wiki.resonite.com/index.php?title=Component:BooleanReferenceDriver&oldid=91235)"

Contents