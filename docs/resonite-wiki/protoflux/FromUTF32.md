# ProtoFlux:FromUTF32

> Source: https://wiki.resonite.com/ProtoFlux:FromUTF32

[ ![](https://wiki.resonite.com/images/1/11/Resonite_Wiki-Icon.png) ](https://wiki.resonite.com/Main_Page "Visit the main page")
Toggle search
Search [ ](https://wiki.resonite.com/Special:Random "Random page")
Toggle menu
[ ![](https://wiki.resonite.com/images/1/11/Resonite_Wiki-Icon.png) ](https://wiki.resonite.com/Main_Page "Visit the main page")
Resonite Wiki
Navigation 
  * [](https://wiki.resonite.com/Special:MyLanguage/Main_Page "Visit the main page \[z\]")
  * [](https://wiki.resonite.com/Special:RecentChanges "A list of recent changes in the wiki \[r\]")
  * [](https://wiki.resonite.com/Special:Random "Load a random page \[x\]")
  * [](https://www.mediawiki.org/wiki/Special:MyLanguage/Help:Contents)
  * [Contributing to the Wiki](https://wiki.resonite.com/Special:MyLanguage/Wiki_Contributions_%26_Translations)
  * [](https://wiki.resonite.com/Special:SpecialPages "A list of all special pages \[q\]")
  * [](https://wiki.resonite.com/Special:Upload "Upload files \[u\]")


Team 
  * [Resonite Team](https://wiki.resonite.com/Special:MyLanguage/Resonite_Team)
  * [Moderation](https://wiki.resonite.com/Special:MyLanguage/Moderation)
  * [Office Hours](https://wiki.resonite.com/Special:MyLanguage/Office_Hours)
  * [Contact Us](https://wiki.resonite.com/Special:MyLanguage/Contact_Us)


Key Information 
  * [Guidelines and Rules](https://wiki.resonite.com/Special:MyLanguage/Guidelines)
  * [FAQ](https://wiki.resonite.com/Special:MyLanguage/Frequently_Asked_Questions)
  * [How to Help](https://wiki.resonite.com/Special:MyLanguage/How_to_Help)
  * [Branding Information](https://wiki.resonite.com/Special:MyLanguage/Branding)
  * [Roadmap](https://wiki.resonite.com/Special:MyLanguage/Roadmap)
  * [Get your Patreon Rewards](https://wiki.resonite.com/Special:MyLanguage/Patreon_Linking)


notifications 
Toggle personal menu
  * Not logged in


user-interface-preferences 
  * [English](https://wiki.resonite.com/ProtoFlux:FromUTF32)


Personal tools 
  * [](https://wiki.resonite.com/Special:MyTalk "Discussion about edits from this IP address \[n\]")
  * [](https://wiki.resonite.com/Special:MyContributions "A list of edits made from this IP address \[y\]")
  * [](https://wiki.resonite.com/index.php?title=Special:CreateAccount&returnto=ProtoFlux%3AFromUTF32 "You are encouraged to create an account and log in; however, it is not mandatory")
  * [](https://wiki.resonite.com/index.php?title=Special:UserLogin&returnto=ProtoFlux%3AFromUTF32 "You are encouraged to log in; however, it is not mandatory \[o\]")


#  ProtoFlux:FromUTF32
From Resonite Wiki
[](https://wiki.resonite.com/ProtoFlux:FromUTF32#top "Back to top \[home\]")
Views 
  * [](https://wiki.resonite.com/ProtoFlux:FromUTF32)
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:FromUTF32&action=edit "This page is protected.
You can view its source \[e\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:FromUTF32&action=history "Past revisions of this page \[h\]")


associated-pages 
  * [ProtoFlux](https://wiki.resonite.com/ProtoFlux:FromUTF32 "View the subject page \[c\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux_talk:FromUTF32&action=edit&redlink=1 "Discussion about the content page \(page does not exist\) \[t\]")


More actions
More 
Tools 
  * [](https://wiki.resonite.com/Special:WhatLinksHere/ProtoFlux:FromUTF32 "A list of all wiki pages that link here \[j\]")
  * [](https://wiki.resonite.com/Special:RecentChangesLinked/ProtoFlux:FromUTF32 "Recent changes in pages linked from this page \[k\]")
  * [](javascript:print\(\); "Printable version of this page \[p\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:FromUTF32&oldid=109839 "Permanent link to this revision of this page")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:FromUTF32&action=info "More information about this page")


From UTF32
UTF32
*
Characters
The **From UTF32** node transforms a UTF32 codepoint into its respective UTF32 character. 
## Inputs
### UTF32 ([int](https://wiki.resonite.com/Type:Int "Type:Int"))
The Unicode codepoint, as a decimal integer, to convert. 
## Outputs
### * ([string](https://wiki.resonite.com/Type:String "Type:String"))
The resulting converted character. If the input does not reside within [valid Unicode codepoints](https://en.wikipedia.org/wiki/Unicode#Codespace_and_code_points), a null string will be outputted. 
Note that, while the output of this will be one glyph, it will not always contain one singular `char[](https://wiki.resonite.com/Type:Char "Type:Char")` element. Specifically, when the input extends past the [Basic Multilingual Plane](https://en.wikipedia.org/wiki/Plane_\(Unicode\)#Basic_Multilingual_Plane), a surrogate pair of `char`s will be output. 
## See Also
  * [Microsoft documentation for the `Char.ConvertFromUtf32(Int32)` method.](https://learn.microsoft.com/en-us/dotnet/api/system.char.convertfromutf32)


## Examples
  * [![Four From UTF32 nodes are shown. The first has an input of 65903 and outputs a glyph. The second has an input of 55 and outputs a 7. The third has an input of 1114111 and outputs a nonexistent character, and the fourth has an input of 1114112 and outputs a null string.](https://wiki.resonite.com/images/thumb/8/89/Protoflux_example_From_UTF32_To_UTF32.webp/480px-Protoflux_example_From_UTF32_To_UTF32.webp.png)](https://wiki.resonite.com/File:Protoflux_example_From_UTF32_To_UTF32.webp "Examples of the From UTF32 node and String To UTF32 node, showcasing existing characters, valid but nonexistent characters, and invalid codepoints.")
Examples of the From UTF32 node and [String To UTF32](https://wiki.resonite.com/ProtoFlux:String_To_UTF32 "ProtoFlux:String To UTF32") node, showcasing existing characters, valid but nonexistent characters, and invalid codepoints.


Retrieved from "[https://wiki.resonite.com/index.php?title=ProtoFlux:FromUTF32&oldid=109839](https://wiki.resonite.com/index.php?title=ProtoFlux:FromUTF32&oldid=109839)"
Contents [ Back to top ](https://wiki.resonite.com/ProtoFlux:FromUTF32#top "Back to top \[home\]")
Contents
  * [ 1 Inputs ](https://wiki.resonite.com/ProtoFlux:FromUTF32#Inputs)
    * [ 1.1 UTF32 (int) ](https://wiki.resonite.com/ProtoFlux:FromUTF32#UTF32_\(int\))
  * [ 2 Outputs ](https://wiki.resonite.com/ProtoFlux:FromUTF32#Outputs)
    * [ 2.1 * (string) ](https://wiki.resonite.com/ProtoFlux:FromUTF32#*_\(string\))
  * [ 3 See Also ](https://wiki.resonite.com/ProtoFlux:FromUTF32#See_Also)
  * [ 4 Examples ](https://wiki.resonite.com/ProtoFlux:FromUTF32#Examples)


[Categories](https://wiki.resonite.com/Special:Categories "Special:Categories"): 
  * [ProtoFlux:All](https://wiki.resonite.com/Category:ProtoFlux:All "Category:ProtoFlux:All")
  * [ProtoFlux:Strings:Characters](https://wiki.resonite.com/Category:ProtoFlux:Strings:Characters "Category:ProtoFlux:Strings:Characters")


Last modified
This page was last edited on 21 August 2025, at 00:20.
Resonite Wiki
[Resonite Website](https://resonite.com)
[Resonite Policies](https://resonite.com/policies)
[Resonite on Steam](https://store.steampowered.com/app/2519830/Resonite/)
  * [Privacy policy](https://wiki.resonite.com/Resonite_Wiki:Privacy_policy)
  * [About Resonite Wiki](https://wiki.resonite.com/Resonite_Wiki:About)
  * [Disclaimers](https://wiki.resonite.com/Resonite_Wiki:General_disclaimer)


Content is available under [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/deed.en), unless otherwise specified. 
Resonite is Copyright © Yellow Dog Man Studios s.r.o. 
  * [![Powered by MediaWiki](https://wiki.resonite.com/resources/assets/poweredby_mediawiki_88x31.png)](https://www.mediawiki.org/)


