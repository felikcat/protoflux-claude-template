# ProtoFlux:ToLocalTime

> Source: https://wiki.resonite.com/ProtoFlux:ToLocalTime

To Local Time

DateTime

\*

Time

The `To Local Time` node takes in a DateTime and converts it to local time using your local time offset. This is in accordance to [Universal Time](https://en.wikipedia.org/wiki/Coordinated_Universal_Time).

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

Avoid using [User Time](https://wiki.resonite.com/ProtoFlux:User_Time "ProtoFlux:User Time") with this node, as doing this will show a confusing result. This node is intended to be used with UTC times for converting into a local time.


## Inputs

### DateTime ( [DateTime](https://wiki.resonite.com/Type:DateTime "Type:DateTime"))

The UTC DateTime we want to convert into local time.

## Outputs

### \\* ( [DateTime](https://wiki.resonite.com/Type:DateTime "Type:DateTime"))

Returns the local DateTime.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:ToLocalTime&oldid=110837](https://wiki.resonite.com/index.php?title=ProtoFlux:ToLocalTime&oldid=110837)"

Contents