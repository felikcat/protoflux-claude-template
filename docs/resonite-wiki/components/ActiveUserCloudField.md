# Component:ActiveUserCloudField

> Source: https://wiki.resonite.com/Component:ActiveUserCloudField

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:ActiveUserCloudField&diff=92305) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/f/f8/ActiveUserCloudField%601Component.png/510px-ActiveUserCloudField%601Component.png)](https://wiki.resonite.com/File:ActiveUserCloudField%601Component.png) **Active User Cloud Field<T>** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ActiveUserCloudField** Component binds to the [field](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") specified by `Target`. If `IsLinkedToCloud` is true, it will write the value of the [cloud variable](https://wiki.resonite.com/Cloud_Variables "Cloud Variables") defined by `Path` for the [active user](https://wiki.resonite.com/ProtoFlux:Get_Active_User "ProtoFlux:Get Active User") of the slot it is attached to.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Path` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The [path](https://wiki.resonite.com/Cloud_Variables#Cloud_Variable_Definition "Cloud Variables") of the variable this component will read, for the current [active user](https://wiki.resonite.com/index.php?title=Active_User&action=edit&redlink=1 "Active User (page does not exist)") |
| `IsLinkedToCloud` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | _(Read Only))_ Indicates whether this field was successfully bound to the target variable. |
| `UpdateCloudVariable` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Indicates that this variable should update the value in the cloud when it is written or driven to a different value. |
| `FallbackValue` | **T** | Default value if there is no current active user. If the active user's value isn't set, the definition default will be used instead. |
| `Target` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") <T>>** | The target [field](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") to which the variable value will be written. |

Fields
Collapse

## Usage

For this component to function, the [cloud variable permissions](https://wiki.resonite.com/Cloud_Variables#Permissions "Cloud Variables") must be set to something suitably permissive for it to function properly.

- If the variable should update on the cloud when a user interacts with the object in some way, **Write Permissions** should be set to one of the following:

  - variable\_owner\_unsafe
  - variable\_owner\_only\_contacts\_unsafe 1
  - Anyone 2

- If the variable should update on the cloud when a user interacts with the object in some way, **Read Permissions** should be set to one of the following:

  - variable\_owner\_unsafe
  - variable\_owner\_only\_contacts\_unsafe 3
  - Anyone 4

1\. This permission results in only contacts of the variable owner being able to change a value. It also allows contacts to change each others values, which may not be desired.

2\. This permission is only valid for group variable definitions, and allows anyone to write the value of anyone else, which might have unintended consequences.

3\. This permission results in only contacts of the variable owner being able to read a value, however the value is read by the active user and synced normally to everyone else in a session, making this detail irrelevant.

4\. This permission is only valid for group variable definitions, and allows anyone to read the value of anyone else, however the value is read by the active user and synced normally to everyone else in a session, making this detail irrelevant.

## Examples

Having an item where it changes to the user's color set on the cloud.

## See Also

- [Component:ActiveUserCloudValueVariable](https://wiki.resonite.com/Component:ActiveUserCloudValueVariable "Component:ActiveUserCloudValueVariable")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ActiveUserCloudField&oldid=92305](https://wiki.resonite.com/index.php?title=Component:ActiveUserCloudField&oldid=92305)"

Contents