# ProtoFlux:ParseQuantity

> Source: https://wiki.resonite.com/ProtoFlux:ParseQuantity

Parse Quantity <Type>

Str

Value

DefaultUnit

IsParsed

Quantity

The **Parse Quantity** node takes in a [string](https://wiki.resonite.com/Type:String "Type:String") containing a written quantity value, along with the [string](https://wiki.resonite.com/Type:String "Type:String") of the default unit to assume if no explicit unit is present as part of the input string. It returns the parsed quantity value as a [quantity type](https://wiki.resonite.com/Quantity_Types "Quantity Types") and a [bool](https://wiki.resonite.com/Type:Bool "Type:Bool") indicating wether it parsed successfully.

To create this node, you need to specify a valid [quantity type](https://wiki.resonite.com/Quantity_Types "Quantity Types") for its generic parameter. Examples: `Mass`, `Time`, and `Voltage`.

## Inputs

### Str ( [string](https://wiki.resonite.com/Type:String "Type:String"))

The string to parse.

### DefaultUnit ( [string](https://wiki.resonite.com/Type:String "Type:String"))

The default unit to assume if no unit is present in the input string.

## Outputs

### Value ( [Quantity](https://wiki.resonite.com/Quantity_Types "Quantity Types"))

The parsed quantity value.

### IsParsed ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Wether the input string was parsed successfully.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:ParseQuantity&oldid=110443](https://wiki.resonite.com/index.php?title=ProtoFlux:ParseQuantity&oldid=110443)"

Contents