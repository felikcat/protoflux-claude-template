# Component:TouchablePermissions

> Source: https://wiki.resonite.com/Component:TouchablePermissions

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/4/4c/TouchablePermissionsComponent.png/510px-TouchablePermissionsComponent.png)](https://wiki.resonite.com/File:TouchablePermissionsComponent.png) **Touchable Permissions** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **TouchablePermissions** component is used in worlds to manage what certain roles that users get assigned to can and cannot do.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Tags` | _direct_ **[TagFilter](https://wiki.resonite.com/Type:TagFilter "Type:TagFilter")** | Slot tag object to determine the kinds of tags to filter for the selected roles. |
| `Components` | _direct_ **[ComponentFilter](https://wiki.resonite.com/Type:ComponentFilter "Type:ComponentFilter")** | A component filter that applies to the selected roles. |

Fields
Collapse

## Usage

Found in the world permissions slot. When attaching a new one for granular control, make sure to select the roles you want the filters to apply to. Then make the filters and edits you need. Don't forget to save the world!

## Examples

Found in a default [world](https://wiki.resonite.com/World "World").

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:TouchablePermissions&oldid=95770](https://wiki.resonite.com/index.php?title=Component:TouchablePermissions&oldid=95770)"

Contents