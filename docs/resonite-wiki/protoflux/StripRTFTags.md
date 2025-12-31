# ProtoFlux:StripRTFTags

> Source: https://wiki.resonite.com/ProtoFlux:StripRTFTags

Strip RTF

String

\*

Strings

Strip RTF is a ProtoFlux node that removes [text formatting](https://wiki.resonite.com/Text_Formatting "Text Formatting") tags such as "<size>" "<b>" "<i>" "<u>".

## Inputs

### String ( [String](https://wiki.resonite.com/Type:String "Type:String"))

The string to strip the RTF tags from.

## Outputs

### \\* ( [String](https://wiki.resonite.com/Type:String "Type:String"))

The input string with all text formatting tags removed.

## Examples

[![](https://wiki.resonite.com/images/thumb/c/cc/StripRTF_Tags_Node_Example.png/300px-StripRTF_Tags_Node_Example.png)](https://wiki.resonite.com/File:StripRTF_Tags_Node_Example.png) Strip RTF Tag node clearing formatting tags from a provided string.

The input string of \`<i>Some</i> <color=red>Red Text</color> and <b>BOLD Text</b>\` will output \`Some Red Text and BOLD Text\` without any additional tags.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:StripRTFTags&oldid=110781](https://wiki.resonite.com/index.php?title=ProtoFlux:StripRTFTags&oldid=110781)"

Contents