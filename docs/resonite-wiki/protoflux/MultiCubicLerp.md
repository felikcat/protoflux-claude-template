# ProtoFlux:MultiCubicLerp

> Source: https://wiki.resonite.com/ProtoFlux:MultiCubicLerp

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
  * [English](https://wiki.resonite.com/ProtoFlux:MultiCubicLerp)


Personal tools 
  * [](https://wiki.resonite.com/Special:MyTalk "Discussion about edits from this IP address \[n\]")
  * [](https://wiki.resonite.com/Special:MyContributions "A list of edits made from this IP address \[y\]")
  * [](https://wiki.resonite.com/index.php?title=Special:CreateAccount&returnto=ProtoFlux%3AMultiCubicLerp "You are encouraged to create an account and log in; however, it is not mandatory")
  * [](https://wiki.resonite.com/index.php?title=Special:UserLogin&returnto=ProtoFlux%3AMultiCubicLerp "You are encouraged to log in; however, it is not mandatory \[o\]")


#  ProtoFlux:MultiCubicLerp
From Resonite Wiki
[](https://wiki.resonite.com/ProtoFlux:MultiCubicLerp#top "Back to top \[home\]")
Views 
  * [](https://wiki.resonite.com/ProtoFlux:MultiCubicLerp)
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:MultiCubicLerp&action=edit "This page is protected.
You can view its source \[e\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:MultiCubicLerp&action=history "Past revisions of this page \[h\]")


associated-pages 
  * [ProtoFlux](https://wiki.resonite.com/ProtoFlux:MultiCubicLerp "View the subject page \[c\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux_talk:MultiCubicLerp&action=edit&redlink=1 "Discussion about the content page \(page does not exist\) \[t\]")


More actions
More 
Tools 
  * [](https://wiki.resonite.com/Special:WhatLinksHere/ProtoFlux:MultiCubicLerp "A list of all wiki pages that link here \[j\]")
  * [](https://wiki.resonite.com/Special:RecentChangesLinked/ProtoFlux:MultiCubicLerp "Recent changes in pages linked from this page \[k\]")
  * [](javascript:print\(\); "Printable version of this page \[p\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:MultiCubicLerp&oldid=110291 "Permanent link to this revision of this page")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:MultiCubicLerp&action=info "More information about this page")


Cubic Lerp
Lerp
*
Operands
+
-
Interpolation
The **Multi Cubic Lerp** takes in any number of tangent points ([TangentPointFloat](https://wiki.resonite.com/index.php?title=Type:TangentPointFloat&action=edit&redlink=1 "Type:TangentPointFloat \(page does not exist\)") or [TangentPointDouble](https://wiki.resonite.com/index.php?title=Type:TangentPointDouble&action=edit&redlink=1 "Type:TangentPointDouble \(page does not exist\)")), and a lerp value to travel from start to finish through all of them. This returns the value of a specific point using that lerp value. 
![](https://wiki.resonite.com/images/d/dd/InformationIcon.svg)
The types needed are found using the [Pack Tangent Point](https://wiki.resonite.com/ProtoFlux:Pack_To_Tangent_Point "ProtoFlux:Pack To Tangent Point") nodes. 
This differs from the [Multi Bezier Curve](https://wiki.resonite.com/ProtoFlux:Multi_Bezier_Curve "ProtoFlux:Multi Bezier Curve") node as it attempts to solve a problem with curves, utilizing [Cubic Spline Interpolation](https://en.wikiversity.org/wiki/Cubic_Spline_Interpolation). 
This node is the multi version of the [Cubic Lerp](https://wiki.resonite.com/ProtoFlux:Cubic_Lerp "ProtoFlux:Cubic Lerp") node. 
## Inputs
### Lerp ([float](https://wiki.resonite.com/Type:Float "Type:Float"))
The travel lerp point from start to finish (per lerp input). 
### Operands ([float](https://wiki.resonite.com/Type:Float "Type:Float"))
The lerp inputs. 
## Outputs
### * (Pseudo-Generic)
Returns the value of a specific point along this lerp value. 
## See Also
  * Wikipedia's definition of a [spline interpolation](https://en.wikipedia.org/wiki/Spline_interpolation) & [runge's phenomenon](https://en.wikipedia.org/wiki/Runge%27s_phenomenon).
  * Wikiversity's [Cubic Spline Interpolation](https://en.wikiversity.org/wiki/Cubic_Spline_Interpolation) page.


Retrieved from "[https://wiki.resonite.com/index.php?title=ProtoFlux:MultiCubicLerp&oldid=110291](https://wiki.resonite.com/index.php?title=ProtoFlux:MultiCubicLerp&oldid=110291)"
Contents [ Back to top ](https://wiki.resonite.com/ProtoFlux:MultiCubicLerp#top "Back to top \[home\]")
Contents
  * [ 1 Inputs ](https://wiki.resonite.com/ProtoFlux:MultiCubicLerp#Inputs)
    * [ 1.1 Lerp (float) ](https://wiki.resonite.com/ProtoFlux:MultiCubicLerp#Lerp_\(float\))
    * [ 1.2 Operands (float) ](https://wiki.resonite.com/ProtoFlux:MultiCubicLerp#Operands_\(float\))
  * [ 2 Outputs ](https://wiki.resonite.com/ProtoFlux:MultiCubicLerp#Outputs)
    * [ 2.1 * (Pseudo-Generic) ](https://wiki.resonite.com/ProtoFlux:MultiCubicLerp#*_\(Pseudo-Generic\))
  * [ 3 See Also ](https://wiki.resonite.com/ProtoFlux:MultiCubicLerp#See_Also)


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


