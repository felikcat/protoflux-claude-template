# Component:LookAtUser

> Source: https://wiki.resonite.com/Component:LookAtUser

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:LookAtUser&diff=105308) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/e/ea/LookAtUserComponent.png/510px-LookAtUserComponent.png)](https://wiki.resonite.com/File:LookAtUserComponent.png) **LookAtUser** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **LookAtUser** component drives the rotation specified by `_rotationDrive` to point towards the user specified in `TargetUser`, or the Local User if `TargetAtLocalUser` is checked.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `TargetUser` | **[User](https://wiki.resonite.com/Type:User "Type:User")** | The user to look at, unless _TargetAtLocalUser_ is checked. |
| `TargetAtLocalUser` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Targets the Local User in each client. |
| `SourcePositionOffset` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | Offset from which to calculate the look vector. |
| `Invert` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | The rotated item faces away from the user, instead of towards. |
| `RotationOffset` | **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The degree to which the item is rotated away from the look vector. |
| `PositionSource` | **[LookAtUser.UserNode](https://wiki.resonite.com/Component:LookAtUser#UserNode)** | The UserNode to calculate the look vector from |
| `AroundAxis` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | The rotation is around an arbitrary axis defined in `Axis`. |
| `Axis` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | A unit vector specifying the arbitrary axis to rotate around |
| `_rotationDrive` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | _Automatically Assigned_ \- The FloatQ to be driven by this component. |

Fields
Collapse

## UserNode

| Name | Value | Description |
| --- | --- | --- |
| `Root` | 0 | Component orients to look at the user's root node (Usually user slot) |
| `Head` | 1 | Component orients to look at the user's head node (Usually the top of the neck where the head bends. |
| `View` | 2 | Component orients to look at the user's view point (camera view) only works in local, else will look at the local user regardless of other settings. This may be a bug. |

Values

## Usage

Attach to a slot, and then specify fields. Sometimes the fields like rotation offset and around axis may not adjust orientation as desired. In most cases, simply adding a slot beside the object that should look at another object (EX a piston that is already oriented to look at its target at rest) and then parenting it will achieve the desired effect.

## Examples

Piston constraints (primagen/cyborgs), UI elements, Turrets, limb constraints, and mechanical machines/parts.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:LookAtUser&oldid=105308](https://wiki.resonite.com/index.php?title=Component:LookAtUser&oldid=105308)"

Contents