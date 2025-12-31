# Component:TransformStreamDriver

> Source: https://wiki.resonite.com/Component:TransformStreamDriver

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/5/50/TransformStreamDriverComponent.png/510px-TransformStreamDriverComponent.png)](https://wiki.resonite.com/File:TransformStreamDriverComponent.png) **TransformStreamDriver** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **TransformStreamDriver** is used to convert a stream of position rotation and scale values into drives which can drive slot transforms. It is used internally by the user positioning system.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `PositionStream` | **[ValueStream\`1](https://wiki.resonite.com/index.php?title=Type:ValueStream%601&action=edit&redlink=1 "Type:ValueStream`1 (page does not exist)") < [Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3") >** | The source of float3 values used to position the slot. |
| `RotationStream` | **[ValueStream\`1](https://wiki.resonite.com/index.php?title=Type:ValueStream%601&action=edit&redlink=1 "Type:ValueStream`1 (page does not exist)") < [FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ") >** | The source of floatQ values used to rotate the slot. |
| `ScaleStream` | **[ValueStream\`1](https://wiki.resonite.com/index.php?title=Type:ValueStream%601&action=edit&redlink=1 "Type:ValueStream`1 (page does not exist)") < [Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3") >** | The source of float3 values used to scale the slot. |
| `RootSpaceStream` | **[ReferenceStream\`1](https://wiki.resonite.com/index.php?title=Type:ReferenceStream%601&action=edit&redlink=1 "Type:ReferenceStream`1 (page does not exist)") < [Slot](https://wiki.resonite.com/Type:Slot "Type:Slot") >** | The slot being used for the root space. |
| `Position` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to drive with the streamed in position values. |
| `Rotation` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The field to drive with the streamed in rotation values. |
| `Scale` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to drive with the streamed in scale values. |
| `AllowOffsets` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to allow offsets to the affected slot/object. |
| `ResetStreamsOnDestroy` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to reset the incoming streams upon destroying this slot. |
| `PositionOffset` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3") >** | Offset to the resulting position value this is driving. |
| `RotationOffset` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ") >** | Offset to the resulting rotation value this is driving. |
| `ScaleOffset` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3") >** | Offset to the resulting scale value this is driving. |
| `RunBeforePhysics` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether or not to run before physics. can fix some issues where users fly off of a platform being driven by this component. |

Fields
Collapse

## Examples

Part of the user positioning system and IK.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:TransformStreamDriver&oldid=106585](https://wiki.resonite.com/index.php?title=Component:TransformStreamDriver&oldid=106585)"

Contents