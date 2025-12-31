# ProtoFlux:RandomString

> Source: https://wiki.resonite.com/ProtoFlux:RandomString

Random String

Characters

\*

Length

Random

The **Random String** node takes in a string value and the length, then returns a randomized [string](https://wiki.resonite.com/Type:String "Type:String") value. The string provided acts as a pool of characters, and you can skew the percent chance of a character being selected if there are multiples of the same character.

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This node constantly changes its value every frame, if you want to use this value, make sure to either [Write](https://wiki.resonite.com/ProtoFlux:Write "ProtoFlux:Write") to a [Variable](https://wiki.resonite.com/ProtoFlux:Data_Model_Store "ProtoFlux:Data Model Store") or use it within that frame.


## Inputs

### Characters ( [string](https://wiki.resonite.com/Type:String "Type:String"))

The pool of characters used for the randomization.

### Length ( [int](https://wiki.resonite.com/Type:Int "Type:Int"))

The length of the output string.

## Outputs

### \\* ( [string](https://wiki.resonite.com/Type:String "Type:String"))

The random result.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:RandomString&oldid=110539](https://wiki.resonite.com/index.php?title=ProtoFlux:RandomString&oldid=110539)"

Contents