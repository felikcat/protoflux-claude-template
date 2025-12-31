# Component:ButtonToggle

> Source: https://wiki.resonite.com/Component:ButtonToggle

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:ButtonToggle&diff=90364) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/d/d9/ButtonToggleComponent.png/510px-ButtonToggleComponent.png)](https://wiki.resonite.com/File:ButtonToggleComponent.png) **Button Toggle** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ButtonValueToggle** component can be used to make an [IButton](https://wiki.resonite.com/Type:IButton "Type:IButton") that switches a [boolean](https://wiki.resonite.com/Type:Bool "Type:Bool") value between `true` and `false` every time the button is pressed.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `TargetValue` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >** | The [boolean](https://wiki.resonite.com/Type:Bool "Type:Bool") to invert whenever the button is pressed. |

Fields
Collapse

## Usage

To function, the component simply needs to be attached to a [slot](https://wiki.resonite.com/Slot "Slot") that also has a button component attached to it. From then on, pressing that button will activate the **ButtonToggle**, making it toggle its `TargetValue` from true to false or the other way round.

## Examples

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ButtonToggle&oldid=90364](https://wiki.resonite.com/index.php?title=Component:ButtonToggle&oldid=90364)"

Contents