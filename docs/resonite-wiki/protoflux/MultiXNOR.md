# ProtoFlux:MultiXNOR

> Source: https://wiki.resonite.com/ProtoFlux:MultiXNOR

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
  * [English](https://wiki.resonite.com/ProtoFlux:MultiXNOR)


Personal tools 
  * [](https://wiki.resonite.com/Special:MyTalk "Discussion about edits from this IP address \[n\]")
  * [](https://wiki.resonite.com/Special:MyContributions "A list of edits made from this IP address \[y\]")
  * [](https://wiki.resonite.com/index.php?title=Special:CreateAccount&returnto=ProtoFlux%3AMultiXNOR "You are encouraged to create an account and log in; however, it is not mandatory")
  * [](https://wiki.resonite.com/index.php?title=Special:UserLogin&returnto=ProtoFlux%3AMultiXNOR "You are encouraged to log in; however, it is not mandatory \[o\]")


#  ProtoFlux:MultiXNOR
From Resonite Wiki
[](https://wiki.resonite.com/ProtoFlux:MultiXNOR#top "Back to top \[home\]")
Views 
  * [](https://wiki.resonite.com/ProtoFlux:MultiXNOR)
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:MultiXNOR&action=edit "This page is protected.
You can view its source \[e\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:MultiXNOR&action=history "Past revisions of this page \[h\]")


associated-pages 
  * [ProtoFlux](https://wiki.resonite.com/ProtoFlux:MultiXNOR "View the subject page \[c\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux_talk:MultiXNOR&action=edit&redlink=1 "Discussion about the content page \(page does not exist\) \[t\]")


More actions
More 
Tools 
  * [](https://wiki.resonite.com/Special:WhatLinksHere/ProtoFlux:MultiXNOR "A list of all wiki pages that link here \[j\]")
  * [](https://wiki.resonite.com/Special:RecentChangesLinked/ProtoFlux:MultiXNOR "Recent changes in pages linked from this page \[k\]")
  * [](javascript:print\(\); "Printable version of this page \[p\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:MultiXNOR&oldid=87613 "Permanent link to this revision of this page")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:MultiXNOR&action=info "More information about this page")


XNOR
Operands
*
+
-
Boolean
The **MultiXNOR** node takes in any number of value inputs (either a [bool](https://wiki.resonite.com/Type:Bool "Type:Bool") or a [number](https://wiki.resonite.com/Value_Type "Value Type") value), and functions as both a [logical XNOR](https://en.wikipedia.org/wiki/Logical_biconditional) or bitwise XNOR depending on the type used. 
```
- If odd number of inputs are true, then the result will be false.
- If even number of inputs are true, then the result will be true.

```

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)
The above ruleset is unique to this node and is different compared to the [XNOR](https://wiki.resonite.com/ProtoFlux:XNOR "ProtoFlux:XNOR") node, where the resulting output is simply just checking against 2 inputs. 
## Inputs
### Operands (Pseudo-generic)
The input values to do boolean calculations with. 
## Outputs
### * (Pseudo-generic)
Returns the result of a logical XNOR of all inputs if the node is a [bool](https://wiki.resonite.com/Type:Bool "Type:Bool") type, bitwise XNOR otherwise. 
## See Also
  * Wikipedia's definition of [logical XNOR](https://en.wikipedia.org/wiki/Logical_biconditional) & [xnor gate](https://en.wikipedia.org/wiki/XNOR_gate).


Retrieved from "[https://wiki.resonite.com/index.php?title=ProtoFlux:MultiXNOR&oldid=87613](https://wiki.resonite.com/index.php?title=ProtoFlux:MultiXNOR&oldid=87613)"
Contents [ Back to top ](https://wiki.resonite.com/ProtoFlux:MultiXNOR#top "Back to top \[home\]")
Contents
  * [ 1 Inputs ](https://wiki.resonite.com/ProtoFlux:MultiXNOR#Inputs)
    * [ 1.1 Operands (Pseudo-generic) ](https://wiki.resonite.com/ProtoFlux:MultiXNOR#Operands_\(Pseudo-generic\))
  * [ 2 Outputs ](https://wiki.resonite.com/ProtoFlux:MultiXNOR#Outputs)
    * [ 2.1 * (Pseudo-generic) ](https://wiki.resonite.com/ProtoFlux:MultiXNOR#*_\(Pseudo-generic\))
  * [ 3 See Also ](https://wiki.resonite.com/ProtoFlux:MultiXNOR#See_Also)


[Categories](https://wiki.resonite.com/Special:Categories "Special:Categories"): 
  * [ProtoFlux:All](https://wiki.resonite.com/Category:ProtoFlux:All "Category:ProtoFlux:All")
  * [ProtoFlux:Operators:Boolean](https://wiki.resonite.com/Category:ProtoFlux:Operators:Boolean "Category:ProtoFlux:Operators:Boolean")


Last modified
This page was last edited on 29 June 2024, at 16:51.
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


