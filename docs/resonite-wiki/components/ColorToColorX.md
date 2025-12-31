# Component:ColorToColorX

> Source: https://wiki.resonite.com/Component:ColorToColorX

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/2/28/ColorToColorXComponent.png/510px-ColorToColorXComponent.png)](https://wiki.resonite.com/File:ColorToColorXComponent.png) **Color To Color X** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ColorToColorX** component uses data from a Color and a ColorProfile to drive the value of a ColorX field with optional write back.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `SourceColor` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Color](https://wiki.resonite.com/Type:Color "Type:Color") >>** | The color to convert into a ColorX for `Target` |
| `SourceProfile` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [ColorProfile](https://wiki.resonite.com/Type:ColorProfile "Type:ColorProfile") >>** | The color profile to use for the resulting `Target` |
| `DefaultProfile` | **[ColorProfile](https://wiki.resonite.com/Type:ColorProfile "Type:ColorProfile")** | the ColorProfile to use for `Target` if `SourceProfile` is empty. |
| `Target` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The field to drive with the converted `SourceColor`. |
| `WriteBack` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to allow changes to the field specified by `Target` to go backwards and affect `DefaultProfile` or `SourceProfile`, and `SourceColor`. See [write backs](https://wiki.resonite.com/Drives#Write_Backs "Drives"). |

Fields
Collapse

## Usage

Attach to a slot and provide `SourceColor`. Then provide either `SourceProfile`, or `DefaultProfile`. The component will then drive a ColorX field through `Target`.

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ColorToColorX&oldid=96502](https://wiki.resonite.com/index.php?title=Component:ColorToColorX&oldid=96502)"

Contents