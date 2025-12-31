# ProtoFlux:SetDateTimeKind

> Source: https://wiki.resonite.com/ProtoFlux:SetDateTimeKind

Set Date Time Kind

DateTime

\*

Kind

DateTime

The `Set DateTime Kind` node takes in a [DateTime](https://wiki.resonite.com/Type:DateTime "Type:DateTime") and an [enum](https://wiki.resonite.com/Category:Enums "Category:Enums") [Kind](https://wiki.resonite.com/Type:DateTimeKind "Type:DateTimeKind") of DateTime, then returns the new DateTime value.

![](https://wiki.resonite.com/images/d/dd/InformationIcon.svg)

This at first may not do anything visually, but this in fact does change the kind value, and can be seen when using the [To Unix Seconds](https://wiki.resonite.com/ProtoFlux:To_Unix_Seconds "ProtoFlux:To Unix Seconds") node, showing that it is changing in a point in time rather than offsetting the DateTime.


## Inputs

### DateTime ( [DateTime](https://wiki.resonite.com/Type:DateTime "Type:DateTime"))

The DateTime to change.

### Kind ( [DateTimeKind](https://wiki.resonite.com/Type:DateTimeKind "Type:DateTimeKind"))

The kind to set for this DateTime.

## Outputs

### \\* ( [DateTime](https://wiki.resonite.com/Type:DateTime "Type:DateTime"))

The new DateTime value.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:SetDateTimeKind&oldid=110665](https://wiki.resonite.com/index.php?title=ProtoFlux:SetDateTimeKind&oldid=110665)"

Contents