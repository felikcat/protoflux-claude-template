# Component:KnobControl

> Source: https://wiki.resonite.com/Component:KnobControl

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:KnobControl&diff=91230) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/e/e3/KnobControlComponent.png/510px-KnobControlComponent.png)](https://wiki.resonite.com/File:KnobControlComponent.png) **Knob Control** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

**KnobControl** takes the local rotation of its slot around a specified axis and applies it proportionally to a floating point value.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Target` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | A field to set with the knob's value. |
| `Callback` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | A delegate that is called with the knob's value change. |
| `RotationAxis` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The axis around which to measure the slot's local rotation. |
| `Rate` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The proportional effect of the knob, in values per full (360-degree) rotation. |
| `Min` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The minimum value for the knob. |
| `Max` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The maximum value for the knob. |
| `_lastRotation` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | (internal, read-only) Used in determining the rotational change. |
| `_lastAxis` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | (internal, read-only) Used if the RotationAxis changes. |
| `_lastUser` | **[User](https://wiki.resonite.com/Type:User "Type:User")** | (internal, read-only) The user who last rotated the slot. |

Fields
Collapse

## Usage

As the local rotation of this component's slot changes, the knob's value is updated according to how much it has rotated about the _RotationAxis_. The amount the value changes is determined by the change in rotation (measured in fractions of a full rotation, so for example a change of one degree would be 1/360), multiplied by the _Rate_.

Note that the value field is not driven. This means it is synced to all users, and can be written to at any time.

This component is most useful when coupled with a [Joint](https://wiki.resonite.com/Joint_(Component) "Joint (Component)") to restrict the slot's rotation to be only around the rotation axis.

## Examples

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:KnobControl&oldid=91230](https://wiki.resonite.com/index.php?title=Component:KnobControl&oldid=91230)"

Contents