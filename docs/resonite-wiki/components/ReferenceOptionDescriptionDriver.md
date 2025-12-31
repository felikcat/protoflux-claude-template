# Component:ReferenceOptionDescriptionDriver

> Source: https://wiki.resonite.com/Component:ReferenceOptionDescriptionDriver

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:ReferenceOptionDescriptionDriver&diff=97701) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/6/65/ReferenceOptionDescriptionDriver%601Component.png/510px-ReferenceOptionDescriptionDriver%601Component.png)](https://wiki.resonite.com/File:ReferenceOptionDescriptionDriver%601Component.png) **Reference Option Description Driver\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Reference Option Description Driver** component is used primarily to [drive](https://wiki.resonite.com/Drive "Drive") the parts that make up a [Context Menu Item Source](https://wiki.resonite.com/Component:ContextMenuItemSource "Component:ContextMenuItemSource"). This component along with ContextMenuItemSource is used in [context menus](https://wiki.resonite.com/Context_menu "Context menu") for toggles where the toggle controls a [reference](https://wiki.resonite.com/Reference_Type "Reference Type") like a [slot](https://wiki.resonite.com/Slot "Slot") or object.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Reference` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [SyncRef\`1](https://wiki.resonite.com/Type:SyncRef%601 "Type:SyncRef`1") <T>>** | The reference field to compare against |
| `ForceDeselected` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Forces any context menu item source to change regardless if it is deselected. |
| `Label` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | The string to set to the chosen label in the list of `Options` |
| `Color` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color to set to the chosen color in the list of `Options` |
| `Sprite` | _direct_ **[RefDrive\`1](https://wiki.resonite.com/index.php?title=Type:RefDrive%601&action=edit&redlink=1 "Type:RefDrive`1 (page does not exist)") < [IAssetProvider\`1](https://wiki.resonite.com/Type:IAssetProvider%601 "Type:IAssetProvider`1") < [Sprite](https://wiki.resonite.com/Type:Sprite "Type:Sprite") >>** | The Sprite to set to the chosen Sprite in the list of `Options` |
| `DefaultOption` | _direct_ **[ReferenceOptionDescriptionDriver\`1.Option](https://wiki.resonite.com/Component:ReferenceOptionDescriptionDriver#Option) <T>** | The option to set `Label`, `Color`, and `Sprite` to when `Reference` doesn't match any `ReferenceTarget`s under the list of `Options` |
| `Options` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[ReferenceOptionDescriptionDriver\`1.Option](https://wiki.resonite.com/Component:ReferenceOptionDescriptionDriver#Option) <T>** | The list to search for a `ReferenceTarget` that matches `Reference`. once a match is found, the option's `Label`, `Color`, and `Sprite` is used to drive this section's drive targets of `Label`, `Color`, and `Sprite`. |

Fields
Collapse

## Option

| Name | Type | Description |
| --- | --- | --- |
| `ReferenceTarget` | [SyncRef\`1](https://wiki.resonite.com/Type:SyncRef%601 "Type:SyncRef`1") <T> | The values below should be used if `Reference` is equal to this. |
| `Label` | [String](https://wiki.resonite.com/Type:String "Type:String") | The label to use if `ReferenceTarget` matches `Reference` |
| `Color` | [ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX") | The color to use if `ReferenceTarget` matches `Reference` |
| `Sprite` | [IAssetProvider\`1](https://wiki.resonite.com/Type:IAssetProvider%601 "Type:IAssetProvider`1") < [Sprite](https://wiki.resonite.com/Type:Sprite "Type:Sprite") > | The sprite to use if `ReferenceTarget` matches `Reference` |

Fields

## Usage

This component can be more efficient than using a bunch of [Reference Equality Drivers](https://wiki.resonite.com/Component:ReferenceEqualityDriver "Component:ReferenceEqualityDriver") and generating a number based on such, or using [ProtoFlux](https://wiki.resonite.com/ProtoFlux "ProtoFlux") for a context menu.

## Examples

This is useful for managing toggles where you want to switch things like music and drive the description based on which music asset you chose in your context menu.

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ReferenceOptionDescriptionDriver&oldid=97701](https://wiki.resonite.com/index.php?title=Component:ReferenceOptionDescriptionDriver&oldid=97701)"

Contents