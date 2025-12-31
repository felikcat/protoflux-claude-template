# ProtoFlux:Input

> Source: https://wiki.resonite.com/ProtoFlux:Input

[A bool input](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=InputBool.png "File:InputBool.png") A [bool](https://wiki.resonite.com/Type:Bool "Type:Bool") input.[A float input](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=InputFloat.png "File:InputFloat.png") A [float](https://wiki.resonite.com/Type:Float "Type:Float") input.[a string input](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=InputString.png "File:InputString.png") A [string](https://wiki.resonite.com/Type:String "Type:String") input.

The **Input** node holds a [value](https://wiki.resonite.com/Value_type "Value type") or [reference](https://wiki.resonite.com/Reference_type "Reference type") type that can be output to any other input. Unlike [variables](https://wiki.resonite.com/Category:ProtoFlux:Variables "Category:ProtoFlux:Variables"), these can be directly modified to see instant changes without the need for a [write node](https://wiki.resonite.com/ProtoFlux:Write "ProtoFlux:Write").

![](https://wiki.resonite.com/images/c/c1/SuggestionIcon.svg)

This is similar to [hard-coding](https://en.wikipedia.org/wiki/Hard_coding) values in programming, or when you need [just a number](https://en.wikipedia.org/wiki/Magic_number_(programming)) for debugging or another reason. It is instead recommended to use values from slots [dynamically](https://wiki.resonite.com/Category:ProtoFlux:Variables:DynamicVariables "Category:ProtoFlux:Variables:DynamicVariables") or built in from a [Slot](https://wiki.resonite.com/Slot "Slot"), [Component](https://wiki.resonite.com/Component "Component"), or another [ProtoFlux](https://wiki.resonite.com/ProtoFlux "ProtoFlux") node.


Different types may have different UI interfaces to represent the values they contain, such as [bool](https://wiki.resonite.com/Type:Bool "Type:Bool") will have a check box, numerical values like an [int](https://wiki.resonite.com/Type:Int "Type:Int") and [float](https://wiki.resonite.com/Type:Float "Type:Float") will have a [TextField](https://wiki.resonite.com/Component:TextField "Component:TextField") that takes in only numbers, and [strings](https://wiki.resonite.com/Type:String "Type:String") can take multiple characters.

## Outputs

### \\* (Generic)

The value or reference that will output from this node to be used somewhere else.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:Input&oldid=96306](https://wiki.resonite.com/index.php?title=ProtoFlux:Input&oldid=96306)"

Contents