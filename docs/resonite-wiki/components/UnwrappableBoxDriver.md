# Component:UnwrappableBoxDriver

> Source: https://wiki.resonite.com/Component:UnwrappableBoxDriver

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:UnwrappableBoxDriver&diff=96347) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/0/08/UnwrappableBoxDriverComponent.png/510px-UnwrappableBoxDriverComponent.png)](https://wiki.resonite.com/File:UnwrappableBoxDriverComponent.png) **Unwrappable Box Driver** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **UnwrappableBoxDriver** component makes a 6 sided cube made of individual quads that unwrap themselves into a flat area like a paper box.

A box is auto generated upon attaching the component and fields are auto filled.

This can be used for presents or crates.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Unwrap` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The progress of the unwrap. |
| `SideSize` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The size of each side (a default Quad is 1) |
| `ScaleContent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to scale the side slots and align them to fit as `SideSize`'s value increases. |
| `_side0rotation` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The rotation field of side 0 of the box. |
| `_side1rotation` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The rotation field of side 1 of the box. |
| `_side2rotation` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The rotation field of side 2 of the box. |
| `_side3rotation` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The rotation field of side 3 of the box. |
| `_topRotation` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The rotation field of the top side of the box. |
| `_side0offset` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The position field of side 0 of the box. |
| `_side1offset` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The position field of side 1 of the box. |
| `_side2offset` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The position field of side 2 of the box. |
| `_side3offset` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The position field of side 3 of the box. |
| `_topOffset` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The position field of the top side of the box. |
| `_side0contentOffset` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The position field of the content of side 0 of the box. |
| `_side1contentOffset` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The position field of the content of side 1 of the box. |
| `_side2contentOffset` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The position field of the content of side 2 of the box. |
| `_side3contentOffset` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The position field of the content of side 3 of the box. |
| `_topContentOffset` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The position field of the content of the top side of the box. |
| `_side0contentScale` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The scale field of the content of side 0 of the box. |
| `_side1contentScale` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The scale field of the content of side 1 of the box. |
| `_side2contentScale` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The scale field of the content of side 2 of the box. |
| `_side3contentScale` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The scale field of the content of side 3 of the box. |
| `_bottomContentScale` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The scale field of the content of the bottom side of the box. |
| `_topContentScale` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The scale field of the content of the top side of the box. |

Fields
Collapse

## Usage

Attach to a slot and a box will automatically be generated and setup. The sides can be customized to the user's liking and the `Unwrap` field adjusted or hooked into a driver.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:UnwrappableBoxDriver&oldid=96347](https://wiki.resonite.com/index.php?title=Component:UnwrappableBoxDriver&oldid=96347)"

Contents