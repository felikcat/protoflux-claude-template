# ProtoFlux:MultiSlerp

> Source: https://wiki.resonite.com/ProtoFlux:MultiSlerp

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
  * [English](https://wiki.resonite.com/ProtoFlux:MultiSlerp)


Personal tools 
  * [](https://wiki.resonite.com/Special:MyTalk "Discussion about edits from this IP address \[n\]")
  * [](https://wiki.resonite.com/Special:MyContributions "A list of edits made from this IP address \[y\]")
  * [](https://wiki.resonite.com/index.php?title=Special:CreateAccount&returnto=ProtoFlux%3AMultiSlerp "You are encouraged to create an account and log in; however, it is not mandatory")
  * [](https://wiki.resonite.com/index.php?title=Special:UserLogin&returnto=ProtoFlux%3AMultiSlerp "You are encouraged to log in; however, it is not mandatory \[o\]")


#  ProtoFlux:MultiSlerp
From Resonite Wiki
[](https://wiki.resonite.com/ProtoFlux:MultiSlerp#top "Back to top \[home\]")
Views 
  * [](https://wiki.resonite.com/ProtoFlux:MultiSlerp)
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:MultiSlerp&action=edit "This page is protected.
You can view its source \[e\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:MultiSlerp&action=history "Past revisions of this page \[h\]")


associated-pages 
  * [ProtoFlux](https://wiki.resonite.com/ProtoFlux:MultiSlerp "View the subject page \[c\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux_talk:MultiSlerp&action=edit&redlink=1 "Discussion about the content page \(page does not exist\) \[t\]")


More actions
More 
Tools 
  * [](https://wiki.resonite.com/Special:WhatLinksHere/ProtoFlux:MultiSlerp "A list of all wiki pages that link here \[j\]")
  * [](https://wiki.resonite.com/Special:RecentChangesLinked/ProtoFlux:MultiSlerp "Recent changes in pages linked from this page \[k\]")
  * [](javascript:print\(\); "Printable version of this page \[p\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:MultiSlerp&oldid=110297 "Permanent link to this revision of this page")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:MultiSlerp&action=info "More information about this page")


Slerp
Lerp
*
Operands
+
-
Interpolation
The **Multi Slerp** node takes in any number of slerp points along with a lerp value that represents its point in between those. Then it returns the lerped value over time. 
The "S" part of the slerp stands for "spherical", which means that it deals more with rotations and the values relating to that type of movement ([floatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ") for reference). 
This node is the multi version of the [Slerp](https://wiki.resonite.com/ProtoFlux:Slerp "ProtoFlux:Slerp") node. 
## Inputs
### Lerp ([float](https://wiki.resonite.com/Type:Float "Type:Float"))
The lerp value between the start and end points between all slerps. 
### Operands (Pseudo-Generic)
The slerp values. 
## Outputs
### * (Pseudo-Generic)
Returns the value currently being slerped. 
Retrieved from "[https://wiki.resonite.com/index.php?title=ProtoFlux:MultiSlerp&oldid=110297](https://wiki.resonite.com/index.php?title=ProtoFlux:MultiSlerp&oldid=110297)"
Contents [ Back to top ](https://wiki.resonite.com/ProtoFlux:MultiSlerp#top "Back to top \[home\]")
Contents
  * [ 1 Inputs ](https://wiki.resonite.com/ProtoFlux:MultiSlerp#Inputs)
    * [ 1.1 Lerp (float) ](https://wiki.resonite.com/ProtoFlux:MultiSlerp#Lerp_\(float\))
    * [ 1.2 Operands (Pseudo-Generic) ](https://wiki.resonite.com/ProtoFlux:MultiSlerp#Operands_\(Pseudo-Generic\))
  * [ 2 Outputs ](https://wiki.resonite.com/ProtoFlux:MultiSlerp#Outputs)
    * [ 2.1 * (Pseudo-Generic) ](https://wiki.resonite.com/ProtoFlux:MultiSlerp#*_\(Pseudo-Generic\))


[Categories](https://wiki.resonite.com/Special:Categories "Special:Categories"): 
  * [ProtoFlux:All](https://wiki.resonite.com/Category:ProtoFlux:All "Category:ProtoFlux:All")
  * [ProtoFlux:Math:Interpolation](https://wiki.resonite.com/Category:ProtoFlux:Math:Interpolation "Category:ProtoFlux:Math:Interpolation")


Last modified
This page was last edited on 21 August 2025, at 00:27.
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


