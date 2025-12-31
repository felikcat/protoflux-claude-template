# Component:UserDistanceValueDriver

> Source: https://wiki.resonite.com/Component:UserDistanceValueDriver

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:UserDistanceValueDriver&diff=98210) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/9/99/UserDistanceValueDriver%601Component.png/510px-UserDistanceValueDriver%601Component.png)](https://wiki.resonite.com/File:UserDistanceValueDriver%601Component.png) **User Distance Value Driver\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **UserDistanceValueDriver** switches or flip flops or flips between two different values like a conditional or ternary operator when a user is close to or far away from the slot this component is on. The switch is local.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Node` | **[UserRoot.UserNode](https://wiki.resonite.com/Component:UserRoot#UserNode "Component:UserRoot")** | The user node to check distance from. |
| `Distance` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The distance to use when checking near vs far. |
| `TargetField` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **T** | The field to drive with either `NearValue` or flip to `FarValue` depending on distance. |
| `NearValue` | **T** | The value to use to drive `TargetField` with when the local user `Node` under `Distance` away from this component's slot in global space. |
| `FarValue` | **T** | The value to use to drive `TargetField` with when the local user `Node` over `Distance` away from this component's slot in global space. |

Fields
Collapse

## Usage

Attach to a slot that a distance to the local user for a particular slot in global space needs to be checked for. Then provide values for all the component's fields in order for it to work.

## Examples

Can be used to activate a nameplate visual when the user is close, so the activation based on distance stays local.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:UserDistanceValueDriver&oldid=98210](https://wiki.resonite.com/index.php?title=Component:UserDistanceValueDriver&oldid=98210)"

Contents