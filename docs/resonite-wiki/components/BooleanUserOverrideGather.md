# Component:BooleanUserOverrideGather

> Source: https://wiki.resonite.com/Component:BooleanUserOverrideGather

The **BooleanUserOverrideGather** Component allows storing [Boolean](https://wiki.resonite.com/Type:Bool "Type:Bool") "override" values for each user listed under `_overrides` and [driving](https://wiki.resonite.com/Drive "Drive") the `Target` field. The behavior is similar to [ValueUserOverride](https://wiki.resonite.com/Component:ValueUserOverride "Component:ValueUserOverride") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >, except this component also reports aggregate information about the overrides.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/a/aa/BooleanUserOverrideGatherComponent.png/510px-BooleanUserOverrideGatherComponent.png)](https://wiki.resonite.com/File:BooleanUserOverrideGatherComponent.png) **Boolean User Override Gather** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Default` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | The default value given to `Target` if no suitable override exists in `_overrides`. |
| `CreateOverrideOnWrite` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether an entry in `_overrides` should be created when `Target` is written back. |
| `PersistentOverrides` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether values in `_overrides` should persist when the component is saved. |
| `_overrides` | _[unordered list](https://wiki.resonite.com/Type:SyncBag%601 "Type:SyncBag`1")_ of **[Override](https://wiki.resonite.com/Type:Override "Type:Override") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >** | A Bag of the [Boolean](https://wiki.resonite.com/Type:Bool "Type:Bool") Overrides and the corresponding [UserRef](https://wiki.resonite.com/Type:UserRef "Type:UserRef") they apply to. |
| `Target` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Reference to the field that gets driven to the override value. |
| `Any` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Reports `true` when _any user_ in the session would have their override be `true` (either from the default value or an override). |
| `All` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Reports `true` when _all users_ in the session would have their override be `true` (either from the default value or an override). |
| `None` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Reports `true` when _none of the users_ in the session would have their override be `true` (either from the default value or an override). |
| `TrueCount` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Reports the total count of `true` values for all users in the session. |
| `FalseCount` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Reports the total count of `false` values for all users in the session. |
| `ExcludeHeadless` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to exclude a headless user when doing aggregates and overrides. |

Fields
Collapse

Note that the reporting fields (Any, All, None, TrueCount and FalseCount) count only the values for users _in the sessions_ (including away users and headless servers), but not all the values in the `_overrides` list.

## Override

| Name | Type | Description |
| --- | --- | --- |
| `User` | [UserRef](https://wiki.resonite.com/Type:UserRef "Type:UserRef") | The [User](https://wiki.resonite.com/Type:User "Type:User") that should see `Value`'s content inside of `Target` locally instead of `Default`'s content. |
| `Value` | [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") | The Boolean value that `User` should see target driven to locally. |

Fields

## Behavior

The `_overrides` bag contains a list of users and their associated Boolean values - whenever the local user matches a user entry in the bag, the associated value is driven to `Target`. Otherwise, `Target` is driven to the value in `Default`.

`CreateOverrideOnWrite` allows for new users and values to be added to the bag when the driven value in `Target` is directly or indirectly changed by that user. If it is not enabled, the value in `Target` is not changeable unless the override is added or changed manually from the inspector panel.

Attempting to write to or otherwise cause a discrete entry to a driven field is known as Hooking it. Any Hook to the `Target` value is intercepted by the **BooleanUserOverrideGather** Component and will change the modifying user's entry in the `_overrides` bag. If there is no entry for the user and if `CreateOverrideOnWrite` is enabled, it will create an entry using the set value.

## Examples

## Related Components

- [ValueUserOverride](https://wiki.resonite.com/Component:ValueUserOverride "Component:ValueUserOverride")
- [NumericUserOverrideGather](https://wiki.resonite.com/Component:NumericUserOverrideGather "Component:NumericUserOverrideGather")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:BooleanUserOverrideGather&oldid=93862](https://wiki.resonite.com/index.php?title=Component:BooleanUserOverrideGather&oldid=93862)"

Contents