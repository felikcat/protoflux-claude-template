# ProtoFlux:FormatQuantity

> Source: https://wiki.resonite.com/ProtoFlux:FormatQuantity

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
  * [English](https://wiki.resonite.com/ProtoFlux:FormatQuantity)


Personal tools 
  * [](https://wiki.resonite.com/Special:MyTalk "Discussion about edits from this IP address \[n\]")
  * [](https://wiki.resonite.com/Special:MyContributions "A list of edits made from this IP address \[y\]")
  * [](https://wiki.resonite.com/index.php?title=Special:CreateAccount&returnto=ProtoFlux%3AFormatQuantity "You are encouraged to create an account and log in; however, it is not mandatory")
  * [](https://wiki.resonite.com/index.php?title=Special:UserLogin&returnto=ProtoFlux%3AFormatQuantity "You are encouraged to log in; however, it is not mandatory \[o\]")


#  ProtoFlux:FormatQuantity
From Resonite Wiki
[](https://wiki.resonite.com/ProtoFlux:FormatQuantity#top "Back to top \[home\]")
Views 
  * [](https://wiki.resonite.com/ProtoFlux:FormatQuantity)
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:FormatQuantity&action=edit "This page is protected.
You can view its source \[e\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:FormatQuantity&action=history "Past revisions of this page \[h\]")


associated-pages 
  * [ProtoFlux](https://wiki.resonite.com/ProtoFlux:FormatQuantity "View the subject page \[c\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux_talk:FormatQuantity&action=edit&redlink=1 "Discussion about the content page \(page does not exist\) \[t\]")


More actions
More 
Tools 
  * [](https://wiki.resonite.com/Special:WhatLinksHere/ProtoFlux:FormatQuantity "A list of all wiki pages that link here \[j\]")
  * [](https://wiki.resonite.com/Special:RecentChangesLinked/ProtoFlux:FormatQuantity "Recent changes in pages linked from this page \[k\]")
  * [](javascript:print\(\); "Printable version of this page \[p\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:FormatQuantity&oldid=109823 "Permanent link to this revision of this page")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:FormatQuantity&action=info "More information about this page")


Format Quantity <Type>
Value
*
FormatUnit
FormatNumber
UseLongNames
Quantity
The **Format Quantity** node takes in value as a [quantity type](https://wiki.resonite.com/Quantity_Types "Quantity Types"), the unit in which the quantity should be displayed as a [string](https://wiki.resonite.com/Type:String "Type:String"), as well as wether to use the unit's long name instead of the short form. It returns a formatted [string](https://wiki.resonite.com/Type:String "Type:String") containing the quantity value in the specified unit. 
To create this node, you need to specify a valid [quantity type](https://wiki.resonite.com/Quantity_Types "Quantity Types") for its generic parameter. Examples: `Mass`, `Time`, and `Voltage`. 
## Inputs
### Value ([Quantity](https://wiki.resonite.com/Quantity_Types "Quantity Types"))
The quantity value. 
### FormatUnit ([string](https://wiki.resonite.com/Type:String "Type:String"))
The unit in which the quantity should be displayed. 
### FormatNumber ([string](https://wiki.resonite.com/Type:String "Type:String"))
A format string for the number of the quantity. 
### UseLongNames ([bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))
Wether to use the unit's long name instead of the short form. 
## Outputs
### * ([double](https://wiki.resonite.com/Type:Double "Type:Double"))
The formatted string of that provided unit type. 
Retrieved from "[https://wiki.resonite.com/index.php?title=ProtoFlux:FormatQuantity&oldid=109823](https://wiki.resonite.com/index.php?title=ProtoFlux:FormatQuantity&oldid=109823)"
Contents [ Back to top ](https://wiki.resonite.com/ProtoFlux:FormatQuantity#top "Back to top \[home\]")
Contents
  * [ 1 Inputs ](https://wiki.resonite.com/ProtoFlux:FormatQuantity#Inputs)
    * [ 1.1 Value (Quantity) ](https://wiki.resonite.com/ProtoFlux:FormatQuantity#Value_\(Quantity\))
    * [ 1.2 FormatUnit (string) ](https://wiki.resonite.com/ProtoFlux:FormatQuantity#FormatUnit_\(string\))
    * [ 1.3 FormatNumber (string) ](https://wiki.resonite.com/ProtoFlux:FormatQuantity#FormatNumber_\(string\))
    * [ 1.4 UseLongNames (bool) ](https://wiki.resonite.com/ProtoFlux:FormatQuantity#UseLongNames_\(bool\))
  * [ 2 Outputs ](https://wiki.resonite.com/ProtoFlux:FormatQuantity#Outputs)
    * [ 2.1 * (double) ](https://wiki.resonite.com/ProtoFlux:FormatQuantity#*_\(double\))


[Categories](https://wiki.resonite.com/Special:Categories "Special:Categories"): 
  * [ProtoFlux:All](https://wiki.resonite.com/Category:ProtoFlux:All "Category:ProtoFlux:All")
  * [ProtoFlux:Math:Quantity](https://wiki.resonite.com/Category:ProtoFlux:Math:Quantity "Category:ProtoFlux:Math:Quantity")


Last modified
This page was last edited on 21 August 2025, at 00:19.
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


