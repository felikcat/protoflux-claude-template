# Component:RecordEditForm

> Source: https://wiki.resonite.com/Component:RecordEditForm

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/e/e4/RecordEditFormComponent.png/510px-RecordEditFormComponent.png)](https://wiki.resonite.com/File:RecordEditFormComponent.png) **Record Edit Form** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

See [World](https://wiki.resonite.com/World "World").

The **RecordEditForm** component is used to edit the details and info/metadata for a world.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `_worldOrb` | **[WorldOrb](https://wiki.resonite.com/Component:WorldOrb "Component:WorldOrb")** | The world orb that created this dialog. |
| `_name` | **[TextField](https://wiki.resonite.com/Component:TextField "Component:TextField")** | The field to edit the name of the world. |
| `_description` | **[TextField](https://wiki.resonite.com/Component:TextField "Component:TextField")** | The field to edit the description of the world. |
| `_path` | **[TextField](https://wiki.resonite.com/Component:TextField "Component:TextField")** | The field to edit the path of the world. |
| `_tags` | **[TextField](https://wiki.resonite.com/Component:TextField "Component:TextField")** | The field to edit the tags of the world. |
| `_publicSetting` | **[RecordEditForm.PublicSetting](https://wiki.resonite.com/Component:RecordEditForm#PublicSetting)** | The field to edit the of the world. |
| `_readonly` | **[Checkbox](https://wiki.resonite.com/Component:Checkbox "Component:Checkbox")** | The checkbox to edit the read only property of the world. |
| `_ownerUser` | _direct_ **[UserRef](https://wiki.resonite.com/Type:UserRef "Type:UserRef")** | The field to show the owner of the world. |
| `_privateOptionText` | **[Text](https://wiki.resonite.com/Component:Text "Component:Text")** | The field to show the private options of the world. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `OnCancel:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the cancel button is touched. |
| `OnSave:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the save button is touched. |

Triggers
Collapse

## Usage

See [World](https://wiki.resonite.com/World "World").

## Examples

See [World](https://wiki.resonite.com/World "World").

## See Also

See [World](https://wiki.resonite.com/World "World").

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:RecordEditForm&oldid=106536](https://wiki.resonite.com/index.php?title=Component:RecordEditForm&oldid=106536)"

Contents