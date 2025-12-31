# ProtoFlux:UTCNow

> Source: https://wiki.resonite.com/ProtoFlux:UTCNow

Utc Now

\*

Time

Returns the current time in [UTC](https://en.wikipedia.org/wiki/Coordinated_Universal_Time).

Each evaluation triggers an individual call to [DateTime.UtcNow](https://learn.microsoft.com/en-us/dotnet/api/system.datetime.utcnow).
This means that within a single [Impulse](https://wiki.resonite.com/Impulses "Impulses") it can be evaluated with different values.

This can be used to measure the runtime of impulse based ProtoFlux to sub-millisecond precision.

Since UTC is independent of the local user's timezone it should return approximately the same value on every user.

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

Utc Now is still dependent on the local computer's clock. Differences between users in minutes are somewhat common and in case of incorrectly setup clocks they can reach hours easily. Use [World Time Float](https://wiki.resonite.com/ProtoFlux:World_Time_Float "ProtoFlux:World Time Float") or [World Time Double](https://wiki.resonite.com/ProtoFlux:World_Time_Double "ProtoFlux:World Time Double") for a more consistent time source.


## Outputs

### \\* ( [DateTime](https://wiki.resonite.com/Type:DateTime "Type:DateTime"))

The current time in UTC

## Examples

- [![An example code that also demonstrates how to measure runtime of a ProtoFlux loop.](https://wiki.resonite.com/images/thumb/0/0f/Utc_Now_Demo.png/480px-Utc_Now_Demo.png)](https://wiki.resonite.com/File:Utc_Now_Demo.png "An example code that also demonstrates how to measure runtime of a ProtoFlux loop.")

An example code that also demonstrates how to measure runtime of a ProtoFlux loop.


Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:UTCNow&oldid=110915](https://wiki.resonite.com/index.php?title=ProtoFlux:UTCNow&oldid=110915)"

Contents