# ProtoFlux:GetFingerType

> Source: https://wiki.resonite.com/ProtoFlux:GetFingerType

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
  * [English](https://wiki.resonite.com/ProtoFlux:GetFingerType)


Personal tools 
  * [](https://wiki.resonite.com/Special:MyTalk "Discussion about edits from this IP address \[n\]")
  * [](https://wiki.resonite.com/Special:MyContributions "A list of edits made from this IP address \[y\]")
  * [](https://wiki.resonite.com/index.php?title=Special:CreateAccount&returnto=ProtoFlux%3AGetFingerType "You are encouraged to create an account and log in; however, it is not mandatory")
  * [](https://wiki.resonite.com/index.php?title=Special:UserLogin&returnto=ProtoFlux%3AGetFingerType "You are encouraged to log in; however, it is not mandatory \[o\]")


#  ProtoFlux:GetFingerType
From Resonite Wiki
[](https://wiki.resonite.com/ProtoFlux:GetFingerType#top "Back to top \[home\]")
Views 
  * [](https://wiki.resonite.com/ProtoFlux:GetFingerType)
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:GetFingerType&action=edit "This page is protected.
You can view its source \[e\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:GetFingerType&action=history "Past revisions of this page \[h\]")


associated-pages 
  * [ProtoFlux](https://wiki.resonite.com/ProtoFlux:GetFingerType "View the subject page \[c\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux_talk:GetFingerType&action=edit&redlink=1 "Discussion about the content page \(page does not exist\) \[t\]")


More actions
More 
Tools 
  * [](https://wiki.resonite.com/Special:WhatLinksHere/ProtoFlux:GetFingerType "A list of all wiki pages that link here \[j\]")
  * [](https://wiki.resonite.com/Special:RecentChangesLinked/ProtoFlux:GetFingerType "Recent changes in pages linked from this page \[k\]")
  * [](javascript:print\(\); "Printable version of this page \[p\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:GetFingerType&oldid=109877 "Permanent link to this revision of this page")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:GetFingerType&action=info "More information about this page")


Get Finger Type
Node
*
Body Nodes
Get Finger Segment Type is a ProtoFlux node that returns the [FingerType](https://wiki.resonite.com/Type:FingerType "Type:FingerType") [Enum](https://wiki.resonite.com/Category:Enums "Category:Enums") value that describes the provided Node ([BodyNode](https://wiki.resonite.com/Type:BodyNode "Type:BodyNode")), or -1 if not a finger. 
This is a simplified node version of taking a [BodyNode](https://wiki.resonite.com/Type:BodyNode "Type:BodyNode"), using a [To String](https://wiki.resonite.com/ProtoFlux:To_String "ProtoFlux:To String") node on it, and checking it's name contents for one of the [FingerType](https://wiki.resonite.com/Type:FingerType "Type:FingerType") values also fed to a [To String](https://wiki.resonite.com/ProtoFlux:To_String "ProtoFlux:To String")
## Inputs
### Node ([BodyNode](https://wiki.resonite.com/Type:BodyNode "Type:BodyNode"))
The Body node to check for a finger segment 
## Outputs
### * ([FingerType](https://wiki.resonite.com/Type:FingerSegmentType "Type:FingerSegmentType"))
The finger segment of the provided Node ([BodyNode](https://wiki.resonite.com/Type:BodyNode "Type:BodyNode")). 
## Examples
  * [Example of the Get Finger Type node being used in some ProtoFlux code.](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=Protoflux_example_Get_Finger_Type.webp "File:Protoflux example Get Finger Type.webp")
Example of the Get Finger Type node being used in some ProtoFlux code.


Retrieved from "[https://wiki.resonite.com/index.php?title=ProtoFlux:GetFingerType&oldid=109877](https://wiki.resonite.com/index.php?title=ProtoFlux:GetFingerType&oldid=109877)"
Contents [ Back to top ](https://wiki.resonite.com/ProtoFlux:GetFingerType#top "Back to top \[home\]")
Contents
  * [ 1 Inputs ](https://wiki.resonite.com/ProtoFlux:GetFingerType#Inputs)
    * [ 1.1 Node (BodyNode) ](https://wiki.resonite.com/ProtoFlux:GetFingerType#Node_\(BodyNode\))
  * [ 2 Outputs ](https://wiki.resonite.com/ProtoFlux:GetFingerType#Outputs)
    * [ 2.1 * (FingerType) ](https://wiki.resonite.com/ProtoFlux:GetFingerType#*_\(FingerType\))
  * [ 3 Examples ](https://wiki.resonite.com/ProtoFlux:GetFingerType#Examples)


[Categories](https://wiki.resonite.com/Special:Categories "Special:Categories"): 
  * [Pages with broken file links](https://wiki.resonite.com/Category:Pages_with_broken_file_links "Category:Pages with broken file links")
  * [ProtoFlux:All](https://wiki.resonite.com/Category:ProtoFlux:All "Category:ProtoFlux:All")
  * [ProtoFlux:Avatars:BodyNodes](https://wiki.resonite.com/Category:ProtoFlux:Avatars:BodyNodes "Category:ProtoFlux:Avatars:BodyNodes")


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


