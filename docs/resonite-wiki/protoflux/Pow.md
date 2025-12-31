# ProtoFlux:Pow

> Source: https://wiki.resonite.com/ProtoFlux:Pow

nʸ

N

\*

Power

Math

Pow

Q

\*

Pow

Rotation

The **Pow** node takes in a base number and a power to raise the base to, then returns the result.

![](https://wiki.resonite.com/images/c/c1/SuggestionIcon.svg)

For quick and easy nodes that can square and cube, there are the [Value Square](https://wiki.resonite.com/ProtoFlux:Value_Square "ProtoFlux:Value Square") and [Value Cube](https://wiki.resonite.com/ProtoFlux:Value_Cube "ProtoFlux:Value Cube") nodes.


## Inputs

### N (Pseudo-generic)

The base number for this node.

### Power (Pseudo-generic)

The exponent (or power) for this node.

## Outputs

### \\* (Pseudo-generic)

Returns the result of the base raised to the power.

The following special cases are of note, in order of precedence:

- `N` or `Power` is `NaN`: always `NaN`
- `Power` is `Infinity`
  - `-1 < N < 1`: `0`
  - `N == 1`: `1`
  - `N == -1`: `NaN`
  - `Infinity` otherwise.
- `N < 0 && Power < 0 && Power is not an integer`: `NaN`

`Examples
``Suppose we have the base number 3 and an exponent of 4. This is written as 3⁴.

To calculate 3⁴:

3⁴ = 3 × 3 × 3 × 3 = 81

In this example:

``   The base is 3.
The exponent is 4.
3⁴ is read as "three to the power of four" or "three raised to the fourth power."

`

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:Pow&oldid=88713](https://wiki.resonite.com/index.php?title=ProtoFlux:Pow&oldid=88713)"

Contents