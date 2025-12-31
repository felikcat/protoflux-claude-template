# ProtoFlux:ConstructDateTime

> Source: https://wiki.resonite.com/ProtoFlux:ConstructDateTime

Construct DateTime

Year

\*

Month

Day

Hour

Minute

Second

Millisecond

Kind

DateTime

The `Construct DateTime` node takes in everything needed to create a [DateTime](https://wiki.resonite.com/Type:DateTime "Type:DateTime"), the parts include the `Year`, `Month`, `Day`, `Hour`, `Minute`, `Second`, `Millisecond`, and `Kind`. This gets combined into a newly created DateTime value that can be used.

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This node is wanting numbers that are normally expected from an actual date and time, and giving unexpected values can break this node and will not give you the DateTime that you want. Some examples of unexpected numbers:

- Putting zeros (0) in all fields (specifically in the year, month, and day inputs) will break the node.
- Putting the total length of time or more in the input will break this node (ex: 1000 in milliseconds, 65 in minutes, etc).
- Putting negative numbers into the inputs will break this node.

## Inputs

### Year ( [int](https://wiki.resonite.com/Type:Int "Type:Int"))

The year for creating this DateTime.

### Month ( [int](https://wiki.resonite.com/Type:Int "Type:Int"))

The month for creating this DateTime.

### Day ( [int](https://wiki.resonite.com/Type:Int "Type:Int"))

The day for creating this DateTime.

### Hour ( [int](https://wiki.resonite.com/Type:Int "Type:Int"))

The hour for creating this DateTime.

### Minute ( [int](https://wiki.resonite.com/Type:Int "Type:Int"))

The minute for creating this DateTime.

### Second ( [int](https://wiki.resonite.com/Type:Int "Type:Int"))

The second for creating this DateTime.

### Millisecond ( [int](https://wiki.resonite.com/Type:Int "Type:Int"))

The millisecond for creating this DateTime.

### Kind ( [DateTimeKind](https://wiki.resonite.com/Type:DateTimeKind "Type:DateTimeKind"))

The type of time this is (`Unspecified`, `Utc`, or `Local`)

## Outputs

### \\* ( [DateTime](https://wiki.resonite.com/Type:DateTime "Type:DateTime"))

The newly created DateTime value.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:ConstructDateTime&oldid=109563](https://wiki.resonite.com/index.php?title=ProtoFlux:ConstructDateTime&oldid=109563)"

Contents