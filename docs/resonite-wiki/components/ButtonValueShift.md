# Component:ButtonValueShift

> Source: https://wiki.resonite.com/Component:ButtonValueShift

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:ButtonValueShift&diff=90365) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/f/fe/ButtonValueShift%601Component.png/510px-ButtonValueShift%601Component.png)](https://wiki.resonite.com/File:ButtonValueShift%601Component.png) **Button Value Shift\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ButtonValueShift** component can be used to make an [IButton](https://wiki.resonite.com/Type:IButton "Type:IButton") add the `delta` amount to a [value](https://wiki.resonite.com/Value_Type "Value Type") whenever it is pressed.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `TargetValue` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") <T>** | The value to shift. |
| `Delta` | **T** | By how much `TargetValue` should be shifted on each press. |
| `Min` | **T** | The minimum value that can be shifted to. |
| `Max` | **T** | The maximum value that can be shifted to. |
| `WrapAround` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether or not the value should wrap around to the other extreme when reaching either `Min` or `Max`. |
| `MaxIsExclusive` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | When the current amount is at the value before max, it will stop there, unless wrap around is enabled, which then wraps around from the max value - 1. |

Fields
Collapse

## Usage

To function, the component simply needs to be attached to a [slot](https://wiki.resonite.com/Slot "Slot") that also has a button component attached to it.
From then on, pressing that button will activate the **ButtonValueShift**, making it shift its `TargetValue` by its `Delta`.

## Examples

## Related Issues

It is known that you can go over the maximum by setting the `delta` higher than the max or min values, allowing the output to be outside the ranges provided.

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ButtonValueShift&oldid=90365](https://wiki.resonite.com/index.php?title=Component:ButtonValueShift&oldid=90365)"

Contents