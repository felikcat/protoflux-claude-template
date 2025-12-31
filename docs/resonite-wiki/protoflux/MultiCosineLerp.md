# ProtoFlux:MultiCosineLerp

> Source: https://wiki.resonite.com/ProtoFlux:MultiCosineLerp

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
  * [English](https://wiki.resonite.com/ProtoFlux:MultiCosineLerp)


Personal tools 
  * [](https://wiki.resonite.com/Special:MyTalk "Discussion about edits from this IP address \[n\]")
  * [](https://wiki.resonite.com/Special:MyContributions "A list of edits made from this IP address \[y\]")
  * [](https://wiki.resonite.com/index.php?title=Special:CreateAccount&returnto=ProtoFlux%3AMultiCosineLerp "You are encouraged to create an account and log in; however, it is not mandatory")
  * [](https://wiki.resonite.com/index.php?title=Special:UserLogin&returnto=ProtoFlux%3AMultiCosineLerp "You are encouraged to log in; however, it is not mandatory \[o\]")


#  ProtoFlux:MultiCosineLerp
From Resonite Wiki
[](https://wiki.resonite.com/ProtoFlux:MultiCosineLerp#top "Back to top \[home\]")
Views 
  * [](https://wiki.resonite.com/ProtoFlux:MultiCosineLerp)
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:MultiCosineLerp&action=edit "This page is protected.
You can view its source \[e\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:MultiCosineLerp&action=history "Past revisions of this page \[h\]")


associated-pages 
  * [ProtoFlux](https://wiki.resonite.com/ProtoFlux:MultiCosineLerp "View the subject page \[c\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux_talk:MultiCosineLerp&action=edit&redlink=1 "Discussion about the content page \(page does not exist\) \[t\]")


More actions
More 
Tools 
  * [](https://wiki.resonite.com/Special:WhatLinksHere/ProtoFlux:MultiCosineLerp "A list of all wiki pages that link here \[j\]")
  * [](https://wiki.resonite.com/Special:RecentChangesLinked/ProtoFlux:MultiCosineLerp "Recent changes in pages linked from this page \[k\]")
  * [](javascript:print\(\); "Printable version of this page \[p\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:MultiCosineLerp&oldid=110289 "Permanent link to this revision of this page")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:MultiCosineLerp&action=info "More information about this page")


Cosine Lerp
Lerp
*
Operands
+
-
Interpolation
The **Multi Cosine Lerp** node takes in any number of curve points along with a lerp value of which it lerps similarly like a [cosine](https://wiki.resonite.com/ProtoFlux:Cos "ProtoFlux:Cos") wave and returning back to the first curve point, then returns the value over time. 
This is clamped, meaning that you are stuck with being in between all provided curve values. 
This node is the multi version of the [Cosine Lerp](https://wiki.resonite.com/ProtoFlux:Cosine_Lerp "ProtoFlux:Cosine Lerp") node. 
## Inputs
### Lerp ([float](https://wiki.resonite.com/Type:Float "Type:Float"))
The travel curve point from start to finish (per curve input). 
### Operands (Pseudo-Generic)
The curve inputs. 
## Outputs
### * (Pseudo-Generic)
Returns the value currently being lerped. 
## Further Reading
### Videos
Load video
YouTube
YouTube might collect personal data. [Privacy Policy](https://www.youtube.com/howyoutubeworks/user-settings/privacy/)
ContinueDismiss
Retrieved from "[https://wiki.resonite.com/index.php?title=ProtoFlux:MultiCosineLerp&oldid=110289](https://wiki.resonite.com/index.php?title=ProtoFlux:MultiCosineLerp&oldid=110289)"
Contents [ Back to top ](https://wiki.resonite.com/ProtoFlux:MultiCosineLerp#top "Back to top \[home\]")
Contents
  * [ 1 Inputs ](https://wiki.resonite.com/ProtoFlux:MultiCosineLerp#Inputs)
    * [ 1.1 Lerp (float) ](https://wiki.resonite.com/ProtoFlux:MultiCosineLerp#Lerp_\(float\))
    * [ 1.2 Operands (Pseudo-Generic) ](https://wiki.resonite.com/ProtoFlux:MultiCosineLerp#Operands_\(Pseudo-Generic\))
  * [ 2 Outputs ](https://wiki.resonite.com/ProtoFlux:MultiCosineLerp#Outputs)
    * [ 2.1 * (Pseudo-Generic) ](https://wiki.resonite.com/ProtoFlux:MultiCosineLerp#*_\(Pseudo-Generic\))
  * [ 3 Further Reading ](https://wiki.resonite.com/ProtoFlux:MultiCosineLerp#Further_Reading)
    * [ 3.1 Videos ](https://wiki.resonite.com/ProtoFlux:MultiCosineLerp#Videos)


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


