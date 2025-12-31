# Component:LabelContentDriver

> Source: https://wiki.resonite.com/Component:LabelContentDriver

Collapse **Component image**

[File:LabelContentDriverComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=LabelContentDriverComponent.png "File:LabelContentDriverComponent.png") **Label Content Driver** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **LabelContentDriver** Component is used to handle driving and updating the visual of labels placed by a [Labeler Tool](https://wiki.resonite.com/Labeler_Tool "Labeler Tool").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `AutoUpdate` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Automatically update the visual per tick |
| `Padding` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | How much padding this label should have from the label's text content. |
| `BaseWidth` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The width of the underline for the text attached to the label. |
| `ContentOrientSpace` | _direct_ **[RootSpace](https://wiki.resonite.com/Type:RootSpace "Type:RootSpace")** | How to orient the text content of this label. |
| `OrientAtLocalUser` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to look at the local user (usually true) |
| `_contentRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The root of the text content for the label this is driving. |
| `_targetPoint` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The target point of the line coming from the underline for the label this is driving. |
| `_contentRotation` | **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The rotation of the content of the label this is driving. |
| `_contentRotationDrive` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The rotation field of the content. |
| `_labelPosition` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The position field of the label. |
| `_labelWidth` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The length field of the label underline. |
| `_lineWidth` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The width field of the line for the label. |
| `_labelRotation` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The rotation field of the label. |
| `_pointPosition` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The target point field for what the label is pointing to. |

Fields
Collapse

## Usage

Not used directly by the user. Used in the [Labeler Tool](https://wiki.resonite.com/Labeler_Tool "Labeler Tool").

## Examples

See [Labeler Tool](https://wiki.resonite.com/Labeler_Tool "Labeler Tool").

## See Also

- [Labeler Tool](https://wiki.resonite.com/Labeler_Tool "Labeler Tool")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:LabelContentDriver&oldid=98946](https://wiki.resonite.com/index.php?title=Component:LabelContentDriver&oldid=98946)"

Contents