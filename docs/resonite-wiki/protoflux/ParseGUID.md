# ProtoFlux:ParseGUID

> Source: https://wiki.resonite.com/ProtoFlux:ParseGUID

Parse GUID

Str

Value

Parsed

GUIDs

The `Parse GUID` node takes in a string, and returns the [GUID](https://en.wikipedia.org/wiki/Universally_unique_identifier) string represented as a [GUID](https://wiki.resonite.com/Type:Guid "Type:Guid") [Type](https://wiki.resonite.com/Type:Type "Type:Type"), and also if it successfully parsed it.

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

It may be tempting to use this node, but there is currently no support for using it in the [Data Model](https://wiki.resonite.com/Data_Model "Data Model"), as seen in [Issue #1294](https://github.com/Yellow-Dog-Man/Resonite-Issues/issues/1294).

[Frooxius](https://wiki.resonite.com/User:Frooxius "User:Frooxius") even mentions that they would favor [Int128](https://wiki.resonite.com/index.php?title=Type:Int128&action=edit&redlink=1 "Type:Int128 (page does not exist)") and [Uint128](https://wiki.resonite.com/index.php?title=Type:Uint128&action=edit&redlink=1 "Type:Uint128 (page does not exist)") over GUIDs due to abuse with them.

## Inputs

### Str ( [string](https://wiki.resonite.com/Type:String "Type:String"))

Takes in a string to parse the GUID.

## Outputs

### Value ( [GUID](https://wiki.resonite.com/Type:Guid "Type:Guid"))

Returns a GUID string.

### Parsed ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Returns if this string is parsed successfully.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:ParseGUID&oldid=110441](https://wiki.resonite.com/index.php?title=ProtoFlux:ParseGUID&oldid=110441)"

Contents