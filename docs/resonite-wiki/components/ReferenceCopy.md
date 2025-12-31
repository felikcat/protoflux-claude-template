# Component:ReferenceCopy

> Source: https://wiki.resonite.com/Component:ReferenceCopy

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:ReferenceCopy&diff=96508) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/a/ab/ReferenceCopy%601Component.png/510px-ReferenceCopy%601Component.png)](https://wiki.resonite.com/File:ReferenceCopy%601Component.png) **Reference Copy\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ReferenceCopy** component is used to copy one reference to another place, driving the target with an write back option.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Source` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [SyncRef\`1](https://wiki.resonite.com/Type:SyncRef%601 "Type:SyncRef`1") <T>>** | The source to copy the Reference from |
| `Target` | _direct_ **[RefDrive\`1](https://wiki.resonite.com/index.php?title=Type:RefDrive%601&action=edit&redlink=1 "Type:RefDrive`1 (page does not exist)") <T>** | The target to drive to the value of `Source` |
| `WriteBack` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | whether to allow changes done to `Target` to change `Source`. See [write backs](https://wiki.resonite.com/Drives#Write_Backs "Drives"). |

Fields
Collapse

## Usage

Drives the target's reference with the source's reference. When using WriteBack, changes made to the Target are local while editing it. When the user is done setting it, it writes via a network sync to change the Source reference. If the Source and Target are the same, the reference will be completely local, and no network sync happens when changing the reference. When using the ReferenceCopy to make fields local like this, joining users will have the host's reference by default.

## Examples

[ReferenceCopy Example](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=ReferenceCopyExample1.png "File:ReferenceCopyExample1.png")
A ReferenceField<slot>'s Reference is being self driven with a WriteBack - making the Reference local, and still changeable. Changes to this reference will be local.

[ReferenceCopy Example](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=ReferenceCopyExample2.png "File:ReferenceCopyExample2.png")
A ReferenceField<slot>'s Reference is being driven to be "hello" from another ReferenceField<slot>'s Reference. The one in pink is the one being driven.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ReferenceCopy&oldid=96508](https://wiki.resonite.com/index.php?title=Component:ReferenceCopy&oldid=96508)"

Contents