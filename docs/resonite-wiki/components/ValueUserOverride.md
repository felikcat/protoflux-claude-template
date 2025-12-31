# Component:ValueUserOverride

> Source: https://wiki.resonite.com/Component:ValueUserOverride

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:ValueUserOverride&diff=97820) which are not marked for translation.

The **ValueUserOverride** Component allows storing "override" values for each user listed under `_overrides` and [driving](https://wiki.resonite.com/Drive "Drive") the `Target` field with them.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/e/ef/ValueUserOverride%601Component.png/510px-ValueUserOverride%601Component.png)](https://wiki.resonite.com/File:ValueUserOverride%601Component.png) **ValueUserOverride** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Default` | **T** | The default value given to `Target` if no suitable override exists in `_overrides`. |
| `CreateOverrideOnWrite` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Creates an entry in `_overrides` when `Target` is written back. |
| `PersistentOverrides` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Values in `_overrides` are stored with the object when it is saved. |
| `_overrides` | _[unordered list](https://wiki.resonite.com/Type:SyncBag%601 "Type:SyncBag`1")_ of **[Override](https://wiki.resonite.com/Type:Override "Type:Override") <T>** | A list of Overrides and the corresponding users they apply to. |
| `Target` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **T** | Target field of the specified type, that gets driven to the override value. |

Fields
Collapse

## Override

| Name | Type | Description |
| --- | --- | --- |
| `User` | [UserRef](https://wiki.resonite.com/Type:UserRef "Type:UserRef") | The [User](https://wiki.resonite.com/Type:User "Type:User") that should see `Value`'s content inside of `Target` locally instead of `Default`'s content |
| `Value` | **T** | The value that `User` should see target driven to locally. |

Fields

## Usage

## Behavior

The `_overrides` bag contains a list of users and their associated values - whenever the local user matches a user entry in the bag, the associated value is driven to `Target`. Otherwise, `Target` is driven to the value in `Default`.

`CreateOverrideOnWrite` allows for new users and values to be added to the bag when the driven value in `Target` is directly or indirectly changed by that user. If it is not enabled, the value in `Target` is not changeable unless the override is added or changed manually from the inspector panel.

Attempting to write to or otherwise cause a discrete entry to a driven field is known as Hooking it. Any Hook to the `Target` value is intercepted by the **ValueUserOverride** Component and will change the modifying user's entry in the `_overrides` bag. If there is no entry for the user and if `CreateOverrideOnWrite` is enabled, it will create an entry using the set value.

## Examples

- [ValueUserOverride for Local World State](https://www.youtube.com/watch?v=aER4oQ9FwSE) by [ProbablePrime](https://wiki.resonite.com/User:ProbablePrime "User:ProbablePrime")

## Related Components

- [BooleanUserOverrideGather](https://wiki.resonite.com/Component:BooleanUserOverrideGather "Component:BooleanUserOverrideGather")
- [NumericUserOverrideGather](https://wiki.resonite.com/Component:NumericUserOverrideGather "Component:NumericUserOverrideGather")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ValueUserOverride&oldid=97820](https://wiki.resonite.com/index.php?title=Component:ValueUserOverride&oldid=97820)"

Contents