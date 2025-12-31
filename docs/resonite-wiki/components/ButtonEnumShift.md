# Component:ButtonEnumShift

> Source: https://wiki.resonite.com/Component:ButtonEnumShift

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:ButtonEnumShift&diff=90353) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/b/b8/ButtonEnumShift%601Component.png/510px-ButtonEnumShift%601Component.png)](https://wiki.resonite.com/File:ButtonEnumShift%601Component.png) **Button Enum Shift\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ButtonEnumShift** component takes in a target [Enum](https://wiki.resonite.com/Enum "Enum") and the amount to shift by (positive numbers are forward, negative numbers are backwards). When an [IButton](https://wiki.resonite.com/Type:IButton "Type:IButton") component on the same [slot](https://wiki.resonite.com/Slot "Slot") is pressed, this component will shift the enum.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `TargetValue` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") <E>** | The target [Enum](https://wiki.resonite.com/Enum "Enum"). |
| `ShiftDelta` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The amount to shift by. |

Fields
Collapse

## Usage

This is used to shift enums by button press.

## Examples

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ButtonEnumShift&oldid=90353](https://wiki.resonite.com/index.php?title=Component:ButtonEnumShift&oldid=90353)"

Contents