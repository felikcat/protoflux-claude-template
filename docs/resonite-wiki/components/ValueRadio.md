# Component:ValueRadio

> Source: https://wiki.resonite.com/Component:ValueRadio

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:ValueRadio&diff=88778) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/4/42/ValueRadio%601Component.png/510px-ValueRadio%601Component.png)](https://wiki.resonite.com/File:ValueRadio%601Component.png) **ValueRadio\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ValueRadio** component is a listener component that activates or deactivates slots using the `CheckVisual` field, based if a `TargetValue` matches the `OptionValue` field. When a match is found, the `CheckVisual` field will be set to true.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `CheckVisual` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | The boolean that is driven to true whenever the `TargetValue` is equal to the `OptionValue` |
| `OptionValue` | **T** | What to set the `TargetValue` to when the button is pressed. |
| `TargetValue` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") <T>>** | The value to set when the button is pressed. |

Fields
Collapse

## Usage

To function, the component simply needs to be attached to a slot that also has a button component attached to it. From then on, pressing that button will activate the ValueRadio, making it set its `TargetValue` to its `OptionValue`, which then also sets its `CheckVisual` to true.

- This is useful for making forms that need one answer from many choices, a set of button that should only have one being active, and anything that requires only one activation from many things.
- the `CheckVisual` field does not just have to be the active of a slot, this can be any [IField](https://wiki.resonite.com/Type:IField "Type:IField") [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"), allowing users to be creative with how they want to structure their component's logic.

## Examples

## Related Issues

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ValueRadio&oldid=88778](https://wiki.resonite.com/index.php?title=Component:ValueRadio&oldid=88778)"

Contents