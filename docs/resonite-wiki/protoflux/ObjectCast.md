# ProtoFlux:ObjectCast

> Source: https://wiki.resonite.com/ProtoFlux:ObjectCast

_HTML Visual replaced by image due to wiki limitations_

[![A picture of an object cast. Looks like a square object with one side a different color than the other, with a split down the middle that has a beveled edge. Though it's just an image so you can't actually feel such bevel in game even with detailed haptics.](https://wiki.resonite.com/images/3/33/ProtoFlux_visuals_Object_Cast.png)](https://wiki.resonite.com/File:ProtoFlux_visuals_Object_Cast.png) An object cast from [IWorldElement](https://wiki.resonite.com/Type:IWorldElement "Type:IWorldElement") to [IField](https://wiki.resonite.com/Type:IField "Type:IField") <int>.

The **Object Cast** casts any [Object](https://wiki.resonite.com/Type:Object "Type:Object") type into any other object type.

## Inputs

### Input (Pseudo-generic)

The object to cast.

### \\* (Pseudo-generic)

The object casted to the resulting type. If the cast can not be done, the resulting object will be `null`. The exact specifications for what types will be correctly cast to what other types is described by [Microsoft's documentation for type-testing operators and cast expressions](https://learn.microsoft.com/en-us/dotnet/csharp/language-reference/operators/type-testing-and-cast), since this node is simply a wrapper around the `as` keyword.

## See Also

- [ProtoFlux:Value Cast](https://wiki.resonite.com/ProtoFlux:Value_Cast "ProtoFlux:Value Cast") for a value version
- [Component:ReferenceCast](https://wiki.resonite.com/Component:ReferenceCast "Component:ReferenceCast") for a component version

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:ObjectCast&oldid=110333](https://wiki.resonite.com/index.php?title=ProtoFlux:ObjectCast&oldid=110333)"

Contents