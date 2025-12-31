# ProtoFlux:FormatString

> Source: https://wiki.resonite.com/ProtoFlux:FormatString

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
  * [English](https://wiki.resonite.com/ProtoFlux:FormatString)


Personal tools 
  * [](https://wiki.resonite.com/Special:MyTalk "Discussion about edits from this IP address \[n\]")
  * [](https://wiki.resonite.com/Special:MyContributions "A list of edits made from this IP address \[y\]")
  * [](https://wiki.resonite.com/index.php?title=Special:CreateAccount&returnto=ProtoFlux%3AFormatString "You are encouraged to create an account and log in; however, it is not mandatory")
  * [](https://wiki.resonite.com/index.php?title=Special:UserLogin&returnto=ProtoFlux%3AFormatString "You are encouraged to log in; however, it is not mandatory \[o\]")


#  ProtoFlux:FormatString
From Resonite Wiki
[](https://wiki.resonite.com/ProtoFlux:FormatString#top "Back to top \[home\]")
Views 
  * [](https://wiki.resonite.com/ProtoFlux:FormatString)
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:FormatString&action=edit "This page is protected.
You can view its source \[e\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:FormatString&action=history "Past revisions of this page \[h\]")


associated-pages 
  * [ProtoFlux](https://wiki.resonite.com/ProtoFlux:FormatString "View the subject page \[c\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux_talk:FormatString&action=edit&redlink=1 "Discussion about the content page \(page does not exist\) \[t\]")


More actions
More 
Tools 
  * [](https://wiki.resonite.com/Special:WhatLinksHere/ProtoFlux:FormatString "A list of all wiki pages that link here \[j\]")
  * [](https://wiki.resonite.com/Special:RecentChangesLinked/ProtoFlux:FormatString "Recent changes in pages linked from this page \[k\]")
  * [](javascript:print\(\); "Printable version of this page \[p\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:FormatString&oldid=109825 "Permanent link to this revision of this page")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:FormatString&action=info "More information about this page")


Format
Format
*
FormatProvider
Parameters
+
-
Formatting
This node simply calls the C# [String.Format](https://learn.microsoft.com/en-us/dotnet/api/system.string.format?view=netframework-4.7.2) function using the provided parameters. It allows you to take a string like "I am a {0} who likes to do {1} while {2}" And populate {0}, {1}, and {2} with values. If you plug any value into the list of inputs for the Parameters, it will auto add a cast node into an [object](https://wiki.resonite.com/Type:Object "Type:Object"). 
For example using the string `"The number {0} is on the {1} hand and the fact it's enabled is {2}."` for Format. Then Plugging in a [float (1.25)](https://wiki.resonite.com/Type:Float "Type:Float") for the first input, Then a [Chirality (Left)](https://wiki.resonite.com/Type:Chirality "Type:Chirality") to the second, then a [Boolean (True)](https://wiki.resonite.com/Type:Bool "Type:Bool") will result in the output `"The number 1.25 is on the Left hand and the fact it's enabled is True."`
## Inputs
### Format ([String](https://wiki.resonite.com/Type:String "Type:String"))
A [composite format string](https://learn.microsoft.com/en-us/dotnet/standard/base-types/composite-formatting). 
### FormatProvider ([IFormatProvider](https://wiki.resonite.com/Type:IFormatProvider "Type:IFormatProvider"))
An object that supplies culture-specific formatting information. 
Nodes that output this type can be found in [Strings/Localization](https://wiki.resonite.com/Category:ProtoFlux:Strings:Localization "Category:ProtoFlux:Strings:Localization")
### Parameters ([Object](https://wiki.resonite.com/Type:Object "Type:Object"))
A list of object-type parameters that can dynamically change this formatted string of text. 
## Outputs
### * ([String](https://wiki.resonite.com/Type:String "Type:String"))
The formatted string. 
Retrieved from "[https://wiki.resonite.com/index.php?title=ProtoFlux:FormatString&oldid=109825](https://wiki.resonite.com/index.php?title=ProtoFlux:FormatString&oldid=109825)"
Contents [ Back to top ](https://wiki.resonite.com/ProtoFlux:FormatString#top "Back to top \[home\]")
Contents
  * [ 1 Inputs ](https://wiki.resonite.com/ProtoFlux:FormatString#Inputs)
    * [ 1.1 Format (String) ](https://wiki.resonite.com/ProtoFlux:FormatString#Format_\(String\))
    * [ 1.2 FormatProvider (IFormatProvider) ](https://wiki.resonite.com/ProtoFlux:FormatString#FormatProvider_\(IFormatProvider\))
    * [ 1.3 Parameters (Object) ](https://wiki.resonite.com/ProtoFlux:FormatString#Parameters_\(Object\))
  * [ 2 Outputs ](https://wiki.resonite.com/ProtoFlux:FormatString#Outputs)
    * [ 2.1 * (String) ](https://wiki.resonite.com/ProtoFlux:FormatString#*_\(String\))


[Categories](https://wiki.resonite.com/Special:Categories "Special:Categories"): 
  * [ProtoFlux:All](https://wiki.resonite.com/Category:ProtoFlux:All "Category:ProtoFlux:All")
  * [ProtoFlux:Strings:Formatting](https://wiki.resonite.com/Category:ProtoFlux:Strings:Formatting "Category:ProtoFlux:Strings:Formatting")


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


