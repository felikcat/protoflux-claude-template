# Component:NumericUserOverrideGather

> Source: https://wiki.resonite.com/Component:NumericUserOverrideGather

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/9/90/NumericUserOverrideGather%601Component.png/510px-NumericUserOverrideGather%601Component.png)](https://wiki.resonite.com/File:NumericUserOverrideGather%601Component.png) **Numeric User Override Gather\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **NumericOverrideGather** component acts the same as a [Component:ValueUserOverride\`1](https://wiki.resonite.com/Component:ValueUserOverride%601 "Component:ValueUserOverride`1") with the key difference being it can get the average, minimum, maximum, and sum of all the values users picked that are still in the session.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Default` | **T** | The default value to drive `Target` with on the user's local machine if they don't have an override in the list of `_overrides`. |
| `CreateOverrideOnWrite` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether changes to `Target` creates a new override or updates the overrides value for that user. |
| `PersistentOverrides` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the `_overrides` list contents are saved when this component is saved. |
| `_overrides` | _[unordered list](https://wiki.resonite.com/Type:SyncBag%601 "Type:SyncBag`1")_ of **[Override](https://wiki.resonite.com/Type:Override "Type:Override") <T>** | A list of overrides for different users. |
| `Target` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **T** | The field to drive with different values for each user's local machine using the `_overrides` list. |
| `Min` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **T** | The minimum value of all the `_overrides` for currently in session users. If a user doesnt have an entry, they are considered to have an entry of `Default`. |
| `Max` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **T** | The maximum value of all the `_overrides` for currently in session users. If a user doesnt have an entry, they are considered to have an entry of `Default`. |
| `Sum` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **T** | The value for if of all the `_overrides` were added together for currently in session users. If a user doesnt have an entry, they are considered to have an entry of `Default`. |
| `Average` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **T** | The average value of all the `_overrides` for currently in session users. If a user doesnt have an entry, they are considered to have an entry of `Default`. |
| `ExcludeHeadless` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether headless client values should be excluded from calculations. |

Fields
Collapse

## Usage

Can be used to check if all users are using the same setting (like saying they're ready for a game round to start) or check the average of what people say the number of jellybeans in a jar is (so that someone can guess the average and get the closest to the answer)

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Component:ValueUserOverride\`1](https://wiki.resonite.com/Component:ValueUserOverride%601 "Component:ValueUserOverride`1")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:NumericUserOverrideGather&oldid=105344](https://wiki.resonite.com/index.php?title=Component:NumericUserOverrideGather&oldid=105344)"

Contents