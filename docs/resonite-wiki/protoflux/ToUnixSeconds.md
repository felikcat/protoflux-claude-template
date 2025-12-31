# ProtoFlux:ToUnixSeconds

> Source: https://wiki.resonite.com/ProtoFlux:ToUnixSeconds

To Unix Seconds

DateTime

\*

Time

The `To Unix Seconds` node takes in a [DateTime](https://wiki.resonite.com/Type:DateTime "Type:DateTime") and returns with the amount of seconds elapsed from that DateTime since January 1st, 1970.

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

Avoid comparing [UTC Now](https://wiki.resonite.com/ProtoFlux:UTC_Now "ProtoFlux:UTC Now") and [User Time](https://wiki.resonite.com/ProtoFlux:User_Time "ProtoFlux:User Time") against each other for validation with this node. It is accurate to say that UTC and local time are different times (hence, time zones), but since they are both _this_ moment in time, the result is the same. This node actually takes a point in time and compares it to the [Unix Epoch](https://en.wikipedia.org/wiki/Unix_time).


## Inputs

### DateTime ( [DateTime](https://wiki.resonite.com/Type:DateTime "Type:DateTime"))

The DateTime to compare against the start of Unix time.

## Outputs

### \\* ( [long](https://wiki.resonite.com/Type:Long "Type:Long"))

Returns the number in seconds between the two points in time (the DateTime provided and the Unix Epoch) represented as a long.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:ToUnixSeconds&oldid=110851](https://wiki.resonite.com/index.php?title=ProtoFlux:ToUnixSeconds&oldid=110851)"

Contents