# ProtoFlux:GetCharacter

> Source: https://wiki.resonite.com/ProtoFlux:GetCharacter

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
  * [English](https://wiki.resonite.com/ProtoFlux:GetCharacter)


Personal tools 
  * [](https://wiki.resonite.com/Special:MyTalk "Discussion about edits from this IP address \[n\]")
  * [](https://wiki.resonite.com/Special:MyContributions "A list of edits made from this IP address \[y\]")
  * [](https://wiki.resonite.com/index.php?title=Special:CreateAccount&returnto=ProtoFlux%3AGetCharacter "You are encouraged to create an account and log in; however, it is not mandatory")
  * [](https://wiki.resonite.com/index.php?title=Special:UserLogin&returnto=ProtoFlux%3AGetCharacter "You are encouraged to log in; however, it is not mandatory \[o\]")


#  ProtoFlux:GetCharacter
From Resonite Wiki
[](https://wiki.resonite.com/ProtoFlux:GetCharacter#top "Back to top \[home\]")
Views 
  * [](https://wiki.resonite.com/ProtoFlux:GetCharacter)
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:GetCharacter&action=edit "This page is protected.
You can view its source \[e\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:GetCharacter&action=history "Past revisions of this page \[h\]")


associated-pages 
  * [ProtoFlux](https://wiki.resonite.com/ProtoFlux:GetCharacter "View the subject page \[c\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux_talk:GetCharacter&action=edit&redlink=1 "Discussion about the content page \(page does not exist\) \[t\]")


More actions
More 
Tools 
  * [](https://wiki.resonite.com/Special:WhatLinksHere/ProtoFlux:GetCharacter "A list of all wiki pages that link here \[j\]")
  * [](https://wiki.resonite.com/Special:RecentChangesLinked/ProtoFlux:GetCharacter "Recent changes in pages linked from this page \[k\]")
  * [](javascript:print\(\); "Printable version of this page \[p\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:GetCharacter&oldid=109863 "Permanent link to this revision of this page")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:GetCharacter&action=info "More information about this page")


Get Character
Str
*
Index
Characters
The **Get Character** node retrieves a character from a given string at a given index. 
## Inputs
### Str ([string](https://wiki.resonite.com/Type:String "Type:String"))
The string to retrieve a character from. 
### Index ([int](https://wiki.resonite.com/Type:Int "Type:Int"))
The 0-indexed character to retrieve from `Str`. 
## Outputs
### * ([char](https://wiki.resonite.com/Type:Char "Type:Char"))
The character from `Str` at index `Index`. If `Index` is either negative or greater than or equal to the [length](https://wiki.resonite.com/ProtoFlux:String_Length "ProtoFlux:String Length") of `Str`, the output will be a character with value `0`. 
![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)
This node deals with individual [chars](https://wiki.resonite.com/Type:Char "Type:Char") of a string, whether by way of indexing a string or by returning a `char`. This may result in unintuitive behavior with strings containing characters that reside outside the [Basic Multilingual Plane](https://en.wikipedia.org/wiki/Plane_\(Unicode\)#Basic_Multilingual_Plane), such as "mismatched" indices or returning an invalid `char`. For more information, see [the type page for String](https://wiki.resonite.com/Type:String "Type:String"). 
## Examples
  * [![A Get Character node has String input "Cheese Mobile" and Index input "4". The resulting output is "s".](https://wiki.resonite.com/images/thumb/b/b8/Protoflux_example_Get_Character_Substring.webp/480px-Protoflux_example_Get_Character_Substring.webp.png)](https://wiki.resonite.com/File:Protoflux_example_Get_Character_Substring.webp "Get Character being used to retrieve a character from a string, as well as its relation to the Substring node.")
Get Character being used to retrieve a character from a string, as well as its relation to the [Substring node](https://wiki.resonite.com/ProtoFlux:Substring "ProtoFlux:Substring").


Retrieved from "[https://wiki.resonite.com/index.php?title=ProtoFlux:GetCharacter&oldid=109863](https://wiki.resonite.com/index.php?title=ProtoFlux:GetCharacter&oldid=109863)"
Contents [ Back to top ](https://wiki.resonite.com/ProtoFlux:GetCharacter#top "Back to top \[home\]")
Contents
  * [ 1 Inputs ](https://wiki.resonite.com/ProtoFlux:GetCharacter#Inputs)
    * [ 1.1 Str (string) ](https://wiki.resonite.com/ProtoFlux:GetCharacter#Str_\(string\))
    * [ 1.2 Index (int) ](https://wiki.resonite.com/ProtoFlux:GetCharacter#Index_\(int\))
  * [ 2 Outputs ](https://wiki.resonite.com/ProtoFlux:GetCharacter#Outputs)
    * [ 2.1 * (char) ](https://wiki.resonite.com/ProtoFlux:GetCharacter#*_\(char\))
  * [ 3 Examples ](https://wiki.resonite.com/ProtoFlux:GetCharacter#Examples)


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


