# ProtoFlux:LocalTransform

> Source: https://wiki.resonite.com/ProtoFlux:LocalTransform

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
  * [English](https://wiki.resonite.com/ProtoFlux:LocalTransform)


Personal tools 
  * [](https://wiki.resonite.com/Special:MyTalk "Discussion about edits from this IP address \[n\]")
  * [](https://wiki.resonite.com/Special:MyContributions "A list of edits made from this IP address \[y\]")
  * [](https://wiki.resonite.com/index.php?title=Special:CreateAccount&returnto=ProtoFlux%3ALocalTransform "You are encouraged to create an account and log in; however, it is not mandatory")
  * [](https://wiki.resonite.com/index.php?title=Special:UserLogin&returnto=ProtoFlux%3ALocalTransform "You are encouraged to log in; however, it is not mandatory \[o\]")


#  ProtoFlux:LocalTransform
From Resonite Wiki
[](https://wiki.resonite.com/ProtoFlux:LocalTransform#top "Back to top \[home\]")
Views 
  * [](https://wiki.resonite.com/ProtoFlux:LocalTransform)
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:LocalTransform&action=edit "This page is protected.
You can view its source \[e\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:LocalTransform&action=history "Past revisions of this page \[h\]")


associated-pages 
  * [ProtoFlux](https://wiki.resonite.com/ProtoFlux:LocalTransform "View the subject page \[c\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux_talk:LocalTransform&action=edit&redlink=1 "Discussion about the content page \(page does not exist\) \[t\]")


More actions
More 
Tools 
  * [](https://wiki.resonite.com/Special:WhatLinksHere/ProtoFlux:LocalTransform "A list of all wiki pages that link here \[j\]")
  * [](https://wiki.resonite.com/Special:RecentChangesLinked/ProtoFlux:LocalTransform "Recent changes in pages linked from this page \[k\]")
  * [](javascript:print\(\); "Printable version of this page \[p\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:LocalTransform&oldid=110241 "Permanent link to this revision of this page")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:LocalTransform&action=info "More information about this page")


Local Transform
*
Position
Rotation
Scale
Transform
The `Local Transform` node outputs the position, rotation and scale of the input slot in [local coordinate space](https://wiki.resonite.com/Coordinate_spaces#Global_vs._Local "Coordinate spaces"), i.e. the slot's transform relative to its parent slot. 
## Inputs
### * ([Slot](https://wiki.resonite.com/Slot "Slot"))
The slot whose local transform is output. 
## Outputs
### Position ([Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3"))
The local position of the provided * ([Slot](https://wiki.resonite.com/Slot "Slot")). 
### Rotation ([FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ"))
The local rotation of the provided * ([Slot](https://wiki.resonite.com/Slot "Slot")). 
### Scale ([Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3"))
The local scale of the provided * ([Slot](https://wiki.resonite.com/Slot "Slot")). 
## Examples
  * [Local transform being used in a moving object code](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=Protoflux_example_local_transform.webp "File:Protoflux example local transform.webp")
Local transform being used in a moving object code


Retrieved from "[https://wiki.resonite.com/index.php?title=ProtoFlux:LocalTransform&oldid=110241](https://wiki.resonite.com/index.php?title=ProtoFlux:LocalTransform&oldid=110241)"
Contents [ Back to top ](https://wiki.resonite.com/ProtoFlux:LocalTransform#top "Back to top \[home\]")
Contents
  * [ 1 Inputs ](https://wiki.resonite.com/ProtoFlux:LocalTransform#Inputs)
    * [ 1.1 * (Slot) ](https://wiki.resonite.com/ProtoFlux:LocalTransform#*_\(Slot\))
  * [ 2 Outputs ](https://wiki.resonite.com/ProtoFlux:LocalTransform#Outputs)
    * [ 2.1 Position (Float3) ](https://wiki.resonite.com/ProtoFlux:LocalTransform#Position_\(Float3\))
    * [ 2.2 Rotation (FloatQ) ](https://wiki.resonite.com/ProtoFlux:LocalTransform#Rotation_\(FloatQ\))
    * [ 2.3 Scale (Float3) ](https://wiki.resonite.com/ProtoFlux:LocalTransform#Scale_\(Float3\))
  * [ 3 Examples ](https://wiki.resonite.com/ProtoFlux:LocalTransform#Examples)


[Categories](https://wiki.resonite.com/Special:Categories "Special:Categories"): 
  * [Pages with broken file links](https://wiki.resonite.com/Category:Pages_with_broken_file_links "Category:Pages with broken file links")
  * [ProtoFlux:All](https://wiki.resonite.com/Category:ProtoFlux:All "Category:ProtoFlux:All")
  * [ProtoFlux:Transform](https://wiki.resonite.com/Category:ProtoFlux:Transform "Category:ProtoFlux:Transform")
  * [ContinuouslyChanging nodes](https://wiki.resonite.com/Category:ContinuouslyChanging_nodes "Category:ContinuouslyChanging nodes")


Last modified
This page was last edited on 21 August 2025, at 00:26.
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


