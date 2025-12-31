# ProtoFlux:FromUTF16

> Source: https://wiki.resonite.com/ProtoFlux:FromUTF16

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
  * [English](https://wiki.resonite.com/ProtoFlux:FromUTF16)


Personal tools 
  * [](https://wiki.resonite.com/Special:MyTalk "Discussion about edits from this IP address \[n\]")
  * [](https://wiki.resonite.com/Special:MyContributions "A list of edits made from this IP address \[y\]")
  * [](https://wiki.resonite.com/index.php?title=Special:CreateAccount&returnto=ProtoFlux%3AFromUTF16 "You are encouraged to create an account and log in; however, it is not mandatory")
  * [](https://wiki.resonite.com/index.php?title=Special:UserLogin&returnto=ProtoFlux%3AFromUTF16 "You are encouraged to log in; however, it is not mandatory \[o\]")


#  ProtoFlux:FromUTF16
From Resonite Wiki
[](https://wiki.resonite.com/ProtoFlux:FromUTF16#top "Back to top \[home\]")
Views 
  * [](https://wiki.resonite.com/ProtoFlux:FromUTF16)
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:FromUTF16&action=edit "This page is protected.
You can view its source \[e\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:FromUTF16&action=history "Past revisions of this page \[h\]")


associated-pages 
  * [ProtoFlux](https://wiki.resonite.com/ProtoFlux:FromUTF16 "View the subject page \[c\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux_talk:FromUTF16&action=edit&redlink=1 "Discussion about the content page \(page does not exist\) \[t\]")


More actions
More 
Tools 
  * [](https://wiki.resonite.com/Special:WhatLinksHere/ProtoFlux:FromUTF16 "A list of all wiki pages that link here \[j\]")
  * [](https://wiki.resonite.com/Special:RecentChangesLinked/ProtoFlux:FromUTF16 "Recent changes in pages linked from this page \[k\]")
  * [](javascript:print\(\); "Printable version of this page \[p\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:FromUTF16&oldid=109837 "Permanent link to this revision of this page")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:FromUTF16&action=info "More information about this page")


From UTF16
UTF16
*
Characters
The **From UTF16** node transforms a 16-bit Unicode codepoint to its corresponding character within the [Basic Multilingual Plane](https://en.wikipedia.org/wiki/Plane_\(Unicode\)#Basic_Multilingual_Plane). 
## Inputs
### UTF16 ([int](https://wiki.resonite.com/Type:Int "Type:Int"))
The Unicode codepoint, as decimal, to convert. This must reside within the Basic Multilingual Plane (`0x0000-0xFFFF`). The output will "wrap around" at every multiple of 65536, essentially having an implicit modulo. 
## Outputs
### * ([char](https://wiki.resonite.com/Type:Char "Type:Char"))
The resulting converted character. 
## Examples
  * [![Three "From UTF16" nodes are shown. The first has the input 19267 and outputs a chinese character. The second has the input "55" and outputs a 7 character. The third has the input "55 + 65536", and also outputs a 7 character.](https://wiki.resonite.com/images/thumb/e/ee/Protoflux_example_From_UTF16.webp/455px-Protoflux_example_From_UTF16.webp.png)](https://wiki.resonite.com/File:Protoflux_example_From_UTF16.webp "Example of using From UTF16 in some ProtoFlux code, showcasing converting both ASCII and non-ASCII characters, as well as the wraparound behavior after 65536.")
Example of using From UTF16 in some ProtoFlux code, showcasing converting both ASCII and non-ASCII characters, as well as the wraparound behavior after 65536.


Retrieved from "[https://wiki.resonite.com/index.php?title=ProtoFlux:FromUTF16&oldid=109837](https://wiki.resonite.com/index.php?title=ProtoFlux:FromUTF16&oldid=109837)"
Contents [ Back to top ](https://wiki.resonite.com/ProtoFlux:FromUTF16#top "Back to top \[home\]")
Contents
  * [ 1 Inputs ](https://wiki.resonite.com/ProtoFlux:FromUTF16#Inputs)
    * [ 1.1 UTF16 (int) ](https://wiki.resonite.com/ProtoFlux:FromUTF16#UTF16_\(int\))
  * [ 2 Outputs ](https://wiki.resonite.com/ProtoFlux:FromUTF16#Outputs)
    * [ 2.1 * (char) ](https://wiki.resonite.com/ProtoFlux:FromUTF16#*_\(char\))
  * [ 3 Examples ](https://wiki.resonite.com/ProtoFlux:FromUTF16#Examples)


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


