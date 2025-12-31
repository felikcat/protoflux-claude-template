# Component:ValueGraphRecorder

> Source: https://wiki.resonite.com/Component:ValueGraphRecorder

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/d/d3/ValueGraphRecorderComponent.png/510px-ValueGraphRecorderComponent.png)](https://wiki.resonite.com/File:ValueGraphRecorderComponent.png) **Value Graph Recorder** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ValueGraphRecorder** component is used to show a graph of values over time with a specified number of points worth of history. As new points are added, the graph is shifted sideways and old points are deleted.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `RecordingUser` | _direct_ **[UserRef](https://wiki.resonite.com/Type:UserRef "Type:UserRef")** | The user handling updates for this component. |
| `SourceValue` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | The field that will be sampled for values. |
| `UpdateInterval` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The interval, in seconds, that the source field will be sampled at. |
| `Points` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The number of samples to retain. |
| `TargetArray` | **[SyncArray\`1](https://wiki.resonite.com/Type:SyncArray%601 "Type:SyncArray`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | The array to store samples in. Typically this will be the Values field in a [StandaloneRectMesh](https://wiki.resonite.com/index.php?title=Compoment:StandaloneRectMesh&action=edit&redlink=1 "Compoment:StandaloneRectMesh (page does not exist)") < [LineGraphMesh](https://wiki.resonite.com/index.php?title=Type:LineGraphMesh&action=edit&redlink=1 "Type:LineGraphMesh (page does not exist)") > |
| `TargetArrayOffset` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Int](https://wiki.resonite.com/Type:Int "Type:Int") >** | The integer field to set with the offset of where in the TargetArray to start showing samples at. |
| `MinRangeAdjustThreshold` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | If a value in the graph goes beyond this value for currently shown samples, adjust the graph minimum value. |
| `MinRangeAdjustMultiplier` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to increase the graph size downwards when adjusting for min value (1 is exactly to where the value edge is, 2 is add 2 times the needed value to show min on the graph. |
| `MaxRangeAdjustThreshold` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | If a value in the graph goes beyond this value for currently shown samples, adjust the graph maximum value. |
| `MaxRangeAdjustMultiplier` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to increase the graph size upwards when adjusting for min value (1 is exactly to where the value edge is, 2 is add 2 times the needed value to show min on the graph. |
| `RangeMin` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | The field to drive with what the minimum range of the graph all points being shown is currently. |
| `RangeMax` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | The field to drive with what the maximum range of the graph all points being shown is currently. |
| `Drive` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to use drive fields to drive target values rather than field pointers. Makes the calculations local. |
| `_arrayDrive` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[SyncArray\`1](https://wiki.resonite.com/Type:SyncArray%601 "Type:SyncArray`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | The field to drive with the set of samples. Typically this will be the Values field in a [StandaloneRectMesh](https://wiki.resonite.com/index.php?title=Compoment:StandaloneRectMesh&action=edit&redlink=1 "Compoment:StandaloneRectMesh (page does not exist)") < [LineGraphMesh](https://wiki.resonite.com/index.php?title=Type:LineGraphMesh&action=edit&redlink=1 "Type:LineGraphMesh (page does not exist)") > |
| `_arrayOffsetDrive` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The integer field to drive with the offset in the TargetArray to start showing samples at. |
| `_rangeMinDrive` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The field to drive with what the minimum range of the graph all points being shown is currently. |
| `_rangeMaxDrive` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The field to drive with what the maximum range of the graph all points being shown is currently. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `WriteValue:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | force a write of a value to the graph rather than waiting on `Interval` |

Triggers
Collapse

## Usage

Attach to a slot and use with a [Component:StandaloneRectMesh](https://wiki.resonite.com/Component:StandaloneRectMesh "Component:StandaloneRectMesh") on a [Component:MeshRenderer](https://wiki.resonite.com/Component:MeshRenderer "Component:MeshRenderer") with a material to view. Use either the fields or drive fields to drive aspects of the graph display for viewing the graph line.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Component:StandaloneRectMesh](https://wiki.resonite.com/Component:StandaloneRectMesh "Component:StandaloneRectMesh")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ValueGraphRecorder&oldid=98112](https://wiki.resonite.com/index.php?title=Component:ValueGraphRecorder&oldid=98112)"

Contents