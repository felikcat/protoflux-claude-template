# ProtoFlux:Log10

> Source: https://wiki.resonite.com/ProtoFlux:Log10

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
  * [English](https://wiki.resonite.com/ProtoFlux:Log10)


Personal tools 
  * [](https://wiki.resonite.com/Special:MyTalk "Discussion about edits from this IP address \[n\]")
  * [](https://wiki.resonite.com/Special:MyContributions "A list of edits made from this IP address \[y\]")
  * [](https://wiki.resonite.com/index.php?title=Special:CreateAccount&returnto=ProtoFlux%3ALog10 "You are encouraged to create an account and log in; however, it is not mandatory")
  * [](https://wiki.resonite.com/index.php?title=Special:UserLogin&returnto=ProtoFlux%3ALog10 "You are encouraged to log in; however, it is not mandatory \[o\]")


#  ProtoFlux:Log10
From Resonite Wiki
[](https://wiki.resonite.com/ProtoFlux:Log10#top "Back to top \[home\]")
Views 
  * [](https://wiki.resonite.com/ProtoFlux:Log10)
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:Log10&action=edit "This page is protected.
You can view its source \[e\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:Log10&action=history "Past revisions of this page \[h\]")


associated-pages 
  * [ProtoFlux](https://wiki.resonite.com/ProtoFlux:Log10 "View the subject page \[c\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux_talk:Log10&action=edit&redlink=1 "Discussion about the content page \(page does not exist\) \[t\]")


More actions
More 
Tools 
  * [](https://wiki.resonite.com/Special:WhatLinksHere/ProtoFlux:Log10 "A list of all wiki pages that link here \[j\]")
  * [](https://wiki.resonite.com/Special:RecentChangesLinked/ProtoFlux:Log10 "Recent changes in pages linked from this page \[k\]")
  * [](javascript:print\(\); "Printable version of this page \[p\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:Log10&oldid=110261 "Permanent link to this revision of this page")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:Log10&action=info "More information about this page")


Log₁₀
N
*
Math
The `Log 10` node takes in a number we are trying to get to and already provides us the base of 10, which is exactly the same as using the [Log N](https://wiki.resonite.com/ProtoFlux:Log_N "ProtoFlux:Log N") node with the base of 10 in the input. This is called the common logarithm, and returns the result of how many times of base 10 to get that number that was provided. 
![](https://wiki.resonite.com/images/d/dd/InformationIcon.svg)
This common logarithm asks a question: What power must 10 be raised to, in order to get x?. 
![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)
Don't get confused when first using this node, as in [Resonite](https://wiki.resonite.com/Resonite "Resonite") currently the visual for this node is incorrect as it shows Logₑ₁₀ when it should show Log₁₀ instead. Please remove this warning after the visual is fixed within Resonite. 
## Inputs
### N (Pseudo-generic)
The number we are searching for using the base 10. 
## Outputs
### * (Pseudo-generic)
Returns the exponent result. 
## Examples
### Example: log⁡₁₀(1000)
```
   Start with the equation:
   log⁡₁₀(1000) = ?

```
```
   Understand the question:
   We're asking: "What power must 10 be raised to, in order to get 1000?"

```
```
   Calculate the power:
   Since 10 × 10 × 10 = 1000 (which is 10³):
   log⁡₁₀(1000) = 3

```

### Example: log⁡₁₀(50)
```
   Start with the equation:
   log⁡₁₀(50) = ?

```
```
   Use the definition:
   We need to find the power to which 10 must be raised to get 50.

```
```
   Using a calculator:
   When you calculate log⁡₁₀(50), you get approximately:
   log⁡₁₀(50) ≈ 1.69897

```
```
   This means:
   10¹.⁶⁹⁸⁹⁷ ≈ 50

```

### Notes
This may be confusing at first, seeing that log⁡₁₀(10) = 1 and log⁡₁₀(100) = 2, but not log⁡₁₀(50) = 1.5 and showing log⁡₁₀(50) ≈ 1.69897 instead. This is called [Logarithmic Scale](https://en.wikipedia.org/wiki/Logarithmic_scale), and is nonlinear. 
## Flux Examples
  * [![Log10 Example 01](https://wiki.resonite.com/images/thumb/1/19/Log10_Example_01.png/480px-Log10_Example_01.png)](https://wiki.resonite.com/File:Log10_Example_01.png "Log10 Example 01")
Log10 Example 01
  * [![Log10 Example 02](https://wiki.resonite.com/images/thumb/f/f0/Log10_Example_02.png/480px-Log10_Example_02.png)](https://wiki.resonite.com/File:Log10_Example_02.png "Log10 Example 02")
Log10 Example 02


Retrieved from "[https://wiki.resonite.com/index.php?title=ProtoFlux:Log10&oldid=110261](https://wiki.resonite.com/index.php?title=ProtoFlux:Log10&oldid=110261)"
Contents [ Back to top ](https://wiki.resonite.com/ProtoFlux:Log10#top "Back to top \[home\]")
Contents
  * [ 1 Inputs ](https://wiki.resonite.com/ProtoFlux:Log10#Inputs)
    * [ 1.1 N (Pseudo-generic) ](https://wiki.resonite.com/ProtoFlux:Log10#N_\(Pseudo-generic\))
  * [ 2 Outputs ](https://wiki.resonite.com/ProtoFlux:Log10#Outputs)
    * [ 2.1 * (Pseudo-generic) ](https://wiki.resonite.com/ProtoFlux:Log10#*_\(Pseudo-generic\))
  * [ 3 Examples ](https://wiki.resonite.com/ProtoFlux:Log10#Examples)
    * [ 3.1 Example: log⁡₁₀(1000) ](https://wiki.resonite.com/ProtoFlux:Log10#Example:_log%E2%81%A1%E2%82%81%E2%82%80\(1000\))
    * [ 3.2 Example: log⁡₁₀(50) ](https://wiki.resonite.com/ProtoFlux:Log10#Example:_log%E2%81%A1%E2%82%81%E2%82%80\(50\))
    * [ 3.3 Notes ](https://wiki.resonite.com/ProtoFlux:Log10#Notes)
  * [ 4 Flux Examples ](https://wiki.resonite.com/ProtoFlux:Log10#Flux_Examples)


[Categories](https://wiki.resonite.com/Special:Categories "Special:Categories"): 
  * [ProtoFlux:All](https://wiki.resonite.com/Category:ProtoFlux:All "Category:ProtoFlux:All")
  * [ProtoFlux:Math](https://wiki.resonite.com/Category:ProtoFlux:Math "Category:ProtoFlux:Math")


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


