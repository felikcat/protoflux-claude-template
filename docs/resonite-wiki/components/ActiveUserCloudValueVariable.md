# Component:ActiveUserCloudValueVariable

> Source: https://wiki.resonite.com/Component:ActiveUserCloudValueVariable

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:ActiveUserCloudValueVariable&diff=92302) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/6/66/ActiveUserCloudValueVariable%601Component.png/510px-ActiveUserCloudValueVariable%601Component.png)](https://wiki.resonite.com/File:ActiveUserCloudValueVariable%601Component.png) **Active User Cloud Value Variable<T>** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ActiveUserCloudValueVariable** component provides a field that is synced to a cloud variable, with the user it is parented under being the owner of the value. This node follows the same rules as [Cloud Variables](https://wiki.resonite.com/Cloud_Variables "Cloud Variables") except that it caches the quickly made changes and then updates the cloud variable with the cached changes as soon as possible using the cloud.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Path` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The [path](https://wiki.resonite.com/Cloud_Variables#Cloud_Variable_Definition "Cloud Variables") of the variable this component will read, for the current [active user](https://wiki.resonite.com/index.php?title=Active_User&action=edit&redlink=1 "Active User (page does not exist)") |
| `IsLinkedToCloud` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | _(Read Only)_ Indicates whether this field was successfully bound to the target variable. |
| `UpdateCloudVariable` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Indicates that this variable should update the value in the cloud when it is written or driven to a different value. |
| `FallbackValue` | **T** | Default value if there is no current active user. If the active user's value isn't set, the definition default will be used instead. |
| `Value` | **T** | The value from the cloud variable. |

Fields
Collapse

## Usage

To use this component, simply add it to a slot underneath a user's hierarchy and set the `Path` to the path of a cloud variable. (make sure that the variable and component are of the same type!)
The component's `Value` field will then be filled with the value from the cloud variable.

## Examples

Having an item where it changes to the user's color set on the cloud.

## See Also

- [Component:ActiveUserCloudField](https://wiki.resonite.com/Component:ActiveUserCloudField "Component:ActiveUserCloudField")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ActiveUserCloudValueVariable&oldid=92302](https://wiki.resonite.com/index.php?title=Component:ActiveUserCloudValueVariable&oldid=92302)"

Contents