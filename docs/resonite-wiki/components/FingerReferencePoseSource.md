# Component:FingerReferencePoseSource

> Source: https://wiki.resonite.com/Component:FingerReferencePoseSource

Collapse **Component image**

[File:FingerReferencePoseSourceComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=FingerReferencePoseSourceComponent.png "File:FingerReferencePoseSourceComponent.png") **Finger Reference Pose Source** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **FingerReferencePoseSource** component is used to read and generate Pose data from the user or its already created bone hiearchy Template. The Slots used in the `Bones` list need to not be null. Every time the Pose data is read from this component as a Finger Pose Source, the current positions and rotations of the slots in `Bones` are used. This component in itself is a [IFingerPoseSourceComponent](https://wiki.resonite.com/Type:IFingerPoseSourceComponent "Type:IFingerPoseSourceComponent").

For more information on finger pose sources, please see [Finger Posing System](https://wiki.resonite.com/Finger_Posing_System "Finger Posing System").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Bones` | _direct_ **[SyncRefDictionary\`2](https://wiki.resonite.com/index.php?title=Type:SyncRefDictionary%602&action=edit&redlink=1 "Type:SyncRefDictionary`2 (page does not exist)") < [BodyNode](https://wiki.resonite.com/Type:BodyNode "Type:BodyNode"), [Slot](https://wiki.resonite.com/Type:Slot "Type:Slot") >** | A list of bones mapped to Fingers to use as the Finger pose source data for this component. The Fingers need to be in the default hand structure. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `AssignFromBipedRig:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Finds a biped rig Component above this component and uses the found Finger bones to fill `Bones`. |
| ``CaptureReference:ButtonEventHandler`1<ReferenceField`1<IFingerPoseSourceComponent>>`` | **[ButtonEventHandler\`1](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler%601&action=edit&redlink=1 "Type:ButtonEventHandler`1 (page does not exist)") < [ReferenceField\`1](https://wiki.resonite.com/Component:ReferenceField%601 "Component:ReferenceField`1") < [IFingerPoseSourceComponent](https://wiki.resonite.com/Type:IFingerPoseSourceComponent "Type:IFingerPoseSourceComponent") >>** | ✓ | Captures the data from the specified [IFingerPoseSource](https://wiki.resonite.com/Type:IFingerPoseSource "Type:IFingerPoseSource") and sets this component's data with it. |
| `CaptureMyLeftHand:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Captures the data from the Left hand of the user that pressed the button and sets this component's data with it. |
| `CaptureMyRightHand:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Captures the data from the right hand of the user that pressed the button and sets this component's data with it. |
| `GenerateDebugVisual:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Generates a Debug visual and Assigns its bones to any item in `Bones` that are missing slots and adds any finger segments that are missing entries in `Bones` |
| `ClearDebugVisual:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Clears the debug visuals of the hand. (WARNING: visuals may be Referenced by `Bones` |
| `GenerateStaticFingerPoseCode:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Generates C# code for making a static Pose. Possibly was added by [Frooxius](https://wiki.resonite.com/User:Frooxius "User:Frooxius") as a way to make code for the poses like fist and point in the defaults quickly. |

Triggers
Collapse

## Usage

Attach to a slot and use either the generate visuals button or assign from biped rig to make a reference armature. Then, it can either be set from the current hand pose of the user (useful for Index Controller users) or can be adjusted manually. The component can then be used as a [IFingerPoseSourceComponent](https://wiki.resonite.com/Type:IFingerPoseSourceComponent "Type:IFingerPoseSourceComponent").

## Examples

[Finger pose reference Frooxius video](https://youtu.be/P5AKqxCgJYo)

## See Also

- [Finger Posing System](https://wiki.resonite.com/Finger_Posing_System "Finger Posing System")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:FingerReferencePoseSource&oldid=97933](https://wiki.resonite.com/index.php?title=Component:FingerReferencePoseSource&oldid=97933)"

Contents