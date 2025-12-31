# Component:UIGrabInstancer

> Source: https://wiki.resonite.com/Component:UIGrabInstancer

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/1/1c/UIGrabInstancer.png/510px-UIGrabInstancer.png)](https://wiki.resonite.com/File:UIGrabInstancer.png) **UIGrabInstancer** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **UIGrabInstancer** component allows [users](https://wiki.resonite.com/User "User") to instance items from [UIX](https://wiki.resonite.com/UIX "UIX") elements from a template a user provides.

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Template` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot that gets duplicated and grabbed when the GrabInstancer is grabbed. |
| `ContainerTemplate` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | Helps let you compose the duplicate |
| `ContainerTemplateInstanceRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | Helps let you compose the duplicate |
| `ActivateRoot` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether or not the GrabInstancer should activate the newly duplicated slot. |
| `EnableGrabbable` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether or not the GrabInstancer should activate any Grabbable component on the newly duplicated slot. |
| `SetInstancePersistent` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >** | Persistence of the instance |
| `ExcludedParts` | _[list](https://wiki.resonite.com/Type:SyncRefList%601 "Type:SyncRefList`1")_ of **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | Slots will be skipped while duplicating |

Fields
Collapse

## Usage

Useful for making copies of items you referenced, but specifically from the [UIX](https://wiki.resonite.com/UIX "UIX") panels you have.

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

The way this component instances the template, will spawn the copied item where the template is. So it is usually recommended to place the template where the instancer is so it is not jarring when attempting to grab a copy of the [Slot](https://wiki.resonite.com/Slot "Slot"). (the other way is to use [ProtoFlux](https://wiki.resonite.com/ProtoFlux "ProtoFlux") to recenter where the user's hand is to adjust for the distance.)


## Examples

## History

The **UIGrabInstancer** was added in [Beta 2024.4.15.1407](https://wiki.resonite.com/Beta_2024.4.15.1407 "Beta 2024.4.15.1407").

## Related Components

- [GrabInstancer](https://wiki.resonite.com/Component:GrabInstancer "Component:GrabInstancer") is similar to this component, but uses the grab feature in [Resonite](https://wiki.resonite.com/Resonite "Resonite") to make a copy of an item template.

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:UIGrabInstancer&oldid=97801](https://wiki.resonite.com/index.php?title=Component:UIGrabInstancer&oldid=97801)"

Contents