# Component:ReferenceRadio

> Source: https://wiki.resonite.com/Component:ReferenceRadio

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:ReferenceRadio&diff=88772) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/9/93/ReferenceRadio%601Component.png/510px-ReferenceRadio%601Component.png)](https://wiki.resonite.com/File:ReferenceRadio%601Component.png) **ReferenceRadio\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ReferenceRadio** component is a listener component that activates or deactivates slots using the `CheckVisual` field, based if a `TargetReference` matches the `OptionReference` field. When a match is found, the `CheckVisual` field will be set to true.

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `CheckVisual` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | The bool that will be set true when there is a match. |
| `OptionReference` | **T** | The reference we are checking a match for, when found, it will trigger this option. |
| `TargetReference` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [SyncRef\`1](https://wiki.resonite.com/Type:SyncRef%601 "Type:SyncRef`1") <T>>** | The thing we are using to check. |

Fields
Collapse

## Usage

- This is useful for making forms that need one answer from many choices, a set of button that should only have one being active, and anything that requires only one activation from many things.
- the `CheckVisual` field does not just have to be the active of a slot, this can be any [IField](https://wiki.resonite.com/Type:IField "Type:IField") [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"), allowing users to be creative with how they want to structure their component's logic.

## Examples

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ReferenceRadio&oldid=88772](https://wiki.resonite.com/index.php?title=Component:ReferenceRadio&oldid=88772)"

Contents