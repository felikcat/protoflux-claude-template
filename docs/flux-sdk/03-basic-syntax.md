<!--
Source: https://flux-sdk.samsmucny.com/ProtoGraph/Basic-Syntax.html
License: CC BY-NC-SA 4.0
Author: Sam (Papaltine) Smucny
-->

# Basic Syntax

## File Structure

ProtoGraph files are UTF-8 encoded and have the `.pg` extension. Each file defines a single module.

Modules have a header and a body. The header includes:
- Module name
- Inputs: Things like sources that will be used by your module
- Outputs: Things like drives that your module produces
- Global definitions: Global references to Froox Engine entities
- Uses: Other modules that your module uses in the body

The body starts after the `where` keyword and contains an expression to be compiled into nodes.

A module can also have directives on lines before the header to provide instructions to the compiler. These lines start with a "#".

Example module:

```
module BasicModule

in  InputX: int

out Output2X: int

where {
    Intermediate = InputX + 5;
    Output2X = InputX + Intermediate;
}
```

## Whitespace

Whitespace in the module header is significant. Each part of the header must be on its own line. Whitespace in the body is not significant. Explicit open/close symbols and delimiters are required to group and separate expressions.

## Comments

`//` indicates the start of a comment. The remainder of the line will not be parsed.

Special documentation comments using `///` above `let` bindings can be used to generate comments in the generated ProtoFlux (for supported packing formats).

## Keywords

ProtoGraph keywords all start with lowercase letters like in `module`, `where`, `let`, and `use`. See the keyword reference for a full list of keywords.

## Names

Names for nodes, modules, and packages use Pascal Case (First letter Capitalized and every word Capitalized) with letters, numbers, and underscores. Names can start with a capital letter or underscore.

When referencing names that are contained in subdirectories, you separate the path parts with `/` like in `Collections/List/NewList`

## Grouping and Delimiters

There are three different grouping symbols and each has a delimiter:

- **( & )** for explicit order of operations and for specifying the arguments to nodes. Arguments separated by commas.

- **{ & }** for grouping a sequence of expressions together in a specific context. Expressions separated by semicolons.

- **[ & ]** for creating a list. Elements separated by commas.

Trailing delimiters are allowed:

```
NormalList = [ 1, 2, 3 ];
MultiLineList = [
    1,
    2,
    3, // trailing delimiter okay
];
ContextExpressionListThatIsFour = {
    Two = 1 + 1;
    Two + Two; // trailing delimiter okay
};
```
