# Component:WorldValueSync

> Source: https://wiki.resonite.com/Component:WorldValueSync

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/9/99/WorldValueSync%601Component.png/510px-WorldValueSync%601Component.png)](https://wiki.resonite.com/File:WorldValueSync%601Component.png) **World Value Sync\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **WorldValueSync** component is used to sync values from world space to user space.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `LocalValue` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") <T>>** | The value to sync. |

Fields
Collapse

## Usage

Not used directly by the user.

## Examples

Used to keep user space visuals for [World Orbs](https://wiki.resonite.com/World_Orb "World Orb") synced in position with world space visuals.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:WorldValueSync&oldid=100825](https://wiki.resonite.com/index.php?title=Component:WorldValueSync&oldid=100825)"

Contents