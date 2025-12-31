# Component:CloudValueVariableDriver

> Source: https://wiki.resonite.com/Component:CloudValueVariableDriver

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:CloudValueVariableDriver&diff=97271) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/d/d4/CloudValueVariableDriver%601Component.png/510px-CloudValueVariableDriver%601Component.png)](https://wiki.resonite.com/File:CloudValueVariableDriver%601Component.png) **CloudValueVariableDriver<T>** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **CloudValueVariableDriver<T>** component drives the `Target` [field](https://wiki.resonite.com/Field "Field") of type **T** with the value of the specified [cloud variable](https://wiki.resonite.com/Cloud_variable "Cloud variable") owned by the local user.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Path` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The [path](https://wiki.resonite.com/Cloud_Variables#Cloud_Variable_Definition "Cloud Variables") of the variable this component will read. |
| `Target` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **T** | The target [field](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") to which the variable value will be written. |
| `IsLinkedToCloud` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | _(Read Only)_ Indicates whether this field was successfully bound to the target variable. |
| `WriteBack` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Updates the value in the cloud when the driven field is changed. See [write backs](https://wiki.resonite.com/Drives#Write_Backs "Drives"). |
| `FallbackValue` | **T** | Default value if the local user does not have a definition for the cloud variable or the local user does not match `OverrideOwner`. |
| `OverrideOwner` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The UserID of the user that made a definition for the variable specified by `Path` or the local user if not specified. |

Fields
Collapse

## Usage

Upon being given a valid cloud variable `Path`, the component will drive the value of the `Target` with the value of the cloud variable owned by the local user. If `OverrideOwner` is specified, the field will only be driven to the value for the user specified in `OverrideOwner`. Otherwise, the field will take the value of the `FallbackValue`.

## Examples

## See Also

- [Cloud Variables](https://wiki.resonite.com/Cloud_Variables "Cloud Variables")
- [Component:CloudValueVariable](https://wiki.resonite.com/Component:CloudValueVariable "Component:CloudValueVariable")
- [Component:CloudValueField](https://wiki.resonite.com/Component:CloudValueField "Component:CloudValueField")
- [Component:ActiveUserCloudField](https://wiki.resonite.com/Component:ActiveUserCloudField "Component:ActiveUserCloudField")
- [Component:ActiveUserCloudValueVariable](https://wiki.resonite.com/Component:ActiveUserCloudValueVariable "Component:ActiveUserCloudValueVariable")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:CloudValueVariableDriver&oldid=97271](https://wiki.resonite.com/index.php?title=Component:CloudValueVariableDriver&oldid=97271)"

Contents