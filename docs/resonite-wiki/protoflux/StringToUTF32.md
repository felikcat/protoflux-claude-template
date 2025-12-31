# ProtoFlux:StringToUTF32

> Source: https://wiki.resonite.com/ProtoFlux:StringToUTF32

String To UTF32

String

\*

Index

Characters

The **String To UTF32** returns the code point ( [UTF-32](https://wiki.resonite.com/UTF-32 "UTF-32") value) of a character or surrogate pair in a [string](https://wiki.resonite.com/Type:String "Type:String").

## Inputs

### String ( [string](https://wiki.resonite.com/Type:String "Type:String"))

The string to retrieve the character or surrogate pair from.

### Index ( [int](https://wiki.resonite.com/Type:Int "Type:Int"))

The 0-indexed character to retrieve from `String`.

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This node deals with individual [chars](https://wiki.resonite.com/Type:Char "Type:Char") of a string, whether by way of indexing a string or by returning a `char`. This may result in unintuitive behavior with strings containing characters that reside outside the [Basic Multilingual Plane](https://en.wikipedia.org/wiki/Plane_(Unicode)#Basic_Multilingual_Plane), such as "mismatched" indices or returning an invalid `char`. For more information, see [the type page for String](https://wiki.resonite.com/Type:String "Type:String").


## Outputs

### \\* ( [int](https://wiki.resonite.com/Type:Int "Type:Int"))

The code point of the character or surrogate pair at the index in the string.

The value `0` is returned instead if one of the following is true:

- `Index` is greater than or equal to the [String Length](https://wiki.resonite.com/ProtoFlux:String_Length "ProtoFlux:String Length").
- `Index` points to a [low surrogate](https://en.wikipedia.org/wiki/Surrogate_code_points#Surrogates).
- `Index` points to a high surrogate without a low surrogate following it.

## See Also

- [Microsoft documentation for the `Char.ConvertToUtf32(String, Int32)` method](https://learn.microsoft.com/en-us/dotnet/api/system.char.converttoutf32#system-char-converttoutf32(system-string-system-int32)).

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:StringToUTF32&oldid=110777](https://wiki.resonite.com/index.php?title=ProtoFlux:StringToUTF32&oldid=110777)"

Contents