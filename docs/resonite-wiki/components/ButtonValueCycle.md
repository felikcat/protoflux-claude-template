# Component:ButtonValueCycle

> Source: https://wiki.resonite.com/Component:ButtonValueCycle

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/7/7c/ButtonValueCycle%601Component.png/510px-ButtonValueCycle%601Component.png)](https://wiki.resonite.com/File:ButtonValueCycle%601Component.png) **Button Value Cycle\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ButtonValueCycle** component holds a list of [values](https://wiki.resonite.com/Value_Types "Value Types") and takes in a `TargetValue` of a provided type. When an [IButton](https://wiki.resonite.com/Type:IButton "Type:IButton") is pressed while this component is on it, this will cycle through the listed values and send the data through the `TargetValue`.

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `TargetValue` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") <T>** | The value data to send outwards. |
| `Values` | _direct_ **[SyncFieldList\`1](https://wiki.resonite.com/Type:SyncFieldList%601 "Type:SyncFieldList`1") <T>** | The list of values to cycle through. |

Fields
Collapse

## Usage

Useful for needing a way to cycle through values of any type.

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ButtonValueCycle&oldid=90359](https://wiki.resonite.com/index.php?title=Component:ButtonValueCycle&oldid=90359)"

Contents