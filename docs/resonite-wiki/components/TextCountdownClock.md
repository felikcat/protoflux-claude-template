# Component:TextCountdownClock

> Source: https://wiki.resonite.com/Component:TextCountdownClock

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/9/90/TextCountdownClockComponent.png/510px-TextCountdownClockComponent.png)](https://wiki.resonite.com/File:TextCountdownClockComponent.png) **Text Countdown Clock** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **TextCountdownClock** component is able to make a countdown till a certain value of T (world time) since a session started. This drives a text field to do so.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `CountdownTime` | **[Double](https://wiki.resonite.com/Type:Double "Type:Double")** | The world time we are counting down to (The world time is zero when a session starts) |
| `AllowNegative` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether negative time can be displayed after the time for the world has been reached. Or to display 0 if false. |
| `TextTarget` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | Text String field to drive with the form of HH:MM:SS based on the value in `CountdownTime`. |

Fields
Collapse

## Usage

This component creates a Text String in the form of HH:MM:SS as a countdown timer based on the difference in the value of T (world time) and the value of CountdownTime.

## Examples

I have a button in my world, that when pressed, uses [ProtoFlux](https://wiki.resonite.com/ProtoFlux "ProtoFlux") to grab T and add 900 to it, then sets that value as countdownTime. Thus I get a timer for 15 minutes.

For example, if T is 1200 and I wanted a 3-minute timer, I would need to set CountdownTime to, 1200 + (3 (min) \* 60 (seconds)), 1380. and it would output a string of 3:00.
Throw that in a Text Field of a Text Render and then you get a Visible Countdown.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:TextCountdownClock&oldid=95720](https://wiki.resonite.com/index.php?title=Component:TextCountdownClock&oldid=95720)"

Contents