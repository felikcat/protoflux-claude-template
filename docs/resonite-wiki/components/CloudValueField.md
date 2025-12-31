# Component:CloudValueField

> Source: https://wiki.resonite.com/Component:CloudValueField

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:CloudValueField&diff=92306) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/2/2a/CloudValueField%601Component.png/510px-CloudValueField%601Component.png)](https://wiki.resonite.com/File:CloudValueField%601Component.png) **CloudValueField<T>** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **CloudValueField<T>** component links a [field](https://wiki.resonite.com/Field "Field") of type **T** to a cloud variable.

For more info on how Cloud Variables work in general, see [Cloud Variables](https://wiki.resonite.com/Cloud_Variables "Cloud Variables").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Path` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The [path](https://wiki.resonite.com/Cloud_Variables#Cloud_Variable_Definition "Cloud Variables") of the variable this component will read. |
| `IsLinkedToCloud` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | _(Read Only)_ Indicates whether this field was successfully bound to the target variable. |
| `VariableOwnerId` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The UserID of the user that made a definition for the variable specified by `Path` |
| `ChangeHandling` | **[CloudVariableChangeMode](https://wiki.resonite.com/Type:CloudVariableChangeMode "Type:CloudVariableChangeMode")** | See [Cloud Variable Change Mode](https://wiki.resonite.com/Type:CloudVariableChangeMode "Type:CloudVariableChangeMode"). |
| `Target` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") <T>>** | The target [field](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") to which the variable value will be written. |

Fields
Collapse

## Usage

Put this component on a slot, and give it a valid cloud variable `Path` and `VariableOwnerId`. When given a `Target`, the contents of the field given to `Target` will auto update with the cloud variable value. Depending on the value of `ChangeHandling` and `VariableOwnerId`, the cloud variable may be updated through this component as well.

This updates as fast as reading/writing cloud variables permits. All the restrictions that apply to cloud variables apply to this component, including permissions and world contexts.

## Examples

## See Also

- [Cloud Variables](https://wiki.resonite.com/Cloud_Variables "Cloud Variables")
- [Component:CloudValueVariable](https://wiki.resonite.com/Component:CloudValueVariable "Component:CloudValueVariable")
- [Component:ActiveUserCloudField](https://wiki.resonite.com/Component:ActiveUserCloudField "Component:ActiveUserCloudField")
- [Component:ActiveUserCloudValueVariable](https://wiki.resonite.com/Component:ActiveUserCloudValueVariable "Component:ActiveUserCloudValueVariable")
- [Component:CloudValueVariableDriver](https://wiki.resonite.com/Component:CloudValueVariableDriver "Component:CloudValueVariableDriver")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:CloudValueField&oldid=92306](https://wiki.resonite.com/index.php?title=Component:CloudValueField&oldid=92306)"

Contents