# Component:ButtonValueSet

> Source: https://wiki.resonite.com/Component:ButtonValueSet

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/1/10/ButtonValueSet%601Component.png/510px-ButtonValueSet%601Component.png)](https://wiki.resonite.com/File:ButtonValueSet%601Component.png) **Button Value Set\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ButtonValueSet** component takes in a [Value Type](https://wiki.resonite.com/Value_Type "Value Type") and a `TargetValue`. When an [IButton](https://wiki.resonite.com/Type:IButton "Type:IButton") is pressed while this component is on the same [slot](https://wiki.resonite.com/Slot "Slot"), this will send the value to the provided `TargetValue`.

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `TargetValue` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") <T>** | The target to send the value outwards. |
| `SetValue` | **T** | The value to set when the button is pressed. |

Fields
Collapse

## Usage

This is similar to the [Write](https://wiki.resonite.com/ProtoFlux:Write "ProtoFlux:Write") [ProtoFlux](https://wiki.resonite.com/ProtoFlux "ProtoFlux") node but as a component instead.

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ButtonValueSet&oldid=90361](https://wiki.resonite.com/index.php?title=Component:ButtonValueSet&oldid=90361)"

Contents