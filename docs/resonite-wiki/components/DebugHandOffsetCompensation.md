# Component:DebugHandOffsetCompensation

> Source: https://wiki.resonite.com/Component:DebugHandOffsetCompensation

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/6/68/DebugHandOffsetCompensationComponent.png/510px-DebugHandOffsetCompensationComponent.png)](https://wiki.resonite.com/File:DebugHandOffsetCompensationComponent.png) **Debug Hand Offset Compensation** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **DebugHandOffsetCompensation** component constantly changes the mapping offsets of the left and right controllers with the values in its fields. These offsets determine how a controller is kept in a consistent orientation to other controllers a user can have.

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This game element is a debug item. Elements like this may be removed at any time without warning, and creations should not rely on it.


## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `LeftHandPosition` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The position offset of the left hand. |
| `LeftHandRotation` | **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The rotation Offset of the left hand. |
| `RightHandPosition` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The position offset of the right hand. |
| `RightHandRotation` | **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The rotation offset of the right hand. |

Fields
Collapse

## Usage

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:DebugHandOffsetCompensation&oldid=96409](https://wiki.resonite.com/index.php?title=Component:DebugHandOffsetCompensation&oldid=96409)"

Contents