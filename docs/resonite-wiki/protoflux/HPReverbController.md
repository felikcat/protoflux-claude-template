# ProtoFlux:HPReverbController

> Source: https://wiki.resonite.com/ProtoFlux:HPReverbController

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
  * [English](https://wiki.resonite.com/ProtoFlux:HPReverbController)


Personal tools 
  * [](https://wiki.resonite.com/Special:MyTalk "Discussion about edits from this IP address \[n\]")
  * [](https://wiki.resonite.com/Special:MyContributions "A list of edits made from this IP address \[y\]")
  * [](https://wiki.resonite.com/index.php?title=Special:CreateAccount&returnto=ProtoFlux%3AHPReverbController "You are encouraged to create an account and log in; however, it is not mandatory")
  * [](https://wiki.resonite.com/index.php?title=Special:UserLogin&returnto=ProtoFlux%3AHPReverbController "You are encouraged to log in; however, it is not mandatory \[o\]")


#  ProtoFlux:HPReverbController
From Resonite Wiki
[](https://wiki.resonite.com/ProtoFlux:HPReverbController#top "Back to top \[home\]")
Views 
  * [](https://wiki.resonite.com/ProtoFlux:HPReverbController)
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:HPReverbController&action=edit "This page is protected.
You can view its source \[e\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:HPReverbController&action=history "Past revisions of this page \[h\]")


associated-pages 
  * [ProtoFlux](https://wiki.resonite.com/ProtoFlux:HPReverbController "View the subject page \[c\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux_talk:HPReverbController&action=edit&redlink=1 "Discussion about the content page \(page does not exist\) \[t\]")


More actions
More 
Tools 
  * [](https://wiki.resonite.com/Special:WhatLinksHere/ProtoFlux:HPReverbController "A list of all wiki pages that link here \[j\]")
  * [](https://wiki.resonite.com/Special:RecentChangesLinked/ProtoFlux:HPReverbController "Recent changes in pages linked from this page \[k\]")
  * [](javascript:print\(\); "Printable version of this page \[p\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:HPReverbController&oldid=109961 "Permanent link to this revision of this page")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:HPReverbController&action=info "More information about this page")


_This article or section is a stub. You can help the Resonite wiki by expanding it._
HPReverb Controller
User
IsActive
Node
Type
BatteryLevel
IsBatteryCharging
AppMenu
ButtonYB
ButtonXA
Grip
GripTouch
GripClick
Joystick
JoystickClick
Trigger
TriggerClick
Controllers
This node provides information provided by HP Reverb controllers. 
  

## Usage
## Examples
## Inputs
### User ([User](https://wiki.resonite.com/User "User"))
The user we are getting controller information from. 
### Node ([Chirality](https://wiki.resonite.com/Type:Chirality "Type:Chirality"))
The controller side to get information from. 
## Outputs
### IsActive ([bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))
Is this controller actively being used right now. 
### Type ([Type](https://wiki.resonite.com/Type:Type "Type:Type"))
The controller type being used. 
### BatteryLevel ([float](https://wiki.resonite.com/Type:Float "Type:Float"))
The battery level of this controller. 
### IsBatteryCharging ([bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))
Is this controller currently charging. 
### AppMenu ([bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))
Is the app menu button pressed right now. 
### ButtonYB ([bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))
Is the Button YB pressed right now. 
### ButtonXA ([bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))
Is the Button XA pressed right now. 
### Grip ([float](https://wiki.resonite.com/Type:Float "Type:Float"))
The amount of how much this controller is being gripped right now. 
### GripTouch ([bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))
Is the controller's grip touched right now. 
### GripClick ([bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))
Is the controller's grip clicked down right now. 
### Joystick ([float2](https://wiki.resonite.com/Type:Float2 "Type:Float2"))
The position of this controller's joystick. 
### JoystickClick ([bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))
Is the controller's joystick clicked down right now. 
### Trigger ([float](https://wiki.resonite.com/Type:Float "Type:Float"))
The amount of how far this controller's trigger is being pressed down currently. 
### TriggerClick ([bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))
Is the controller's trigger being clicked down right now. 
Retrieved from "[https://wiki.resonite.com/index.php?title=ProtoFlux:HPReverbController&oldid=109961](https://wiki.resonite.com/index.php?title=ProtoFlux:HPReverbController&oldid=109961)"
Contents [ Back to top ](https://wiki.resonite.com/ProtoFlux:HPReverbController#top "Back to top \[home\]")
Contents
  * [ 1 Usage ](https://wiki.resonite.com/ProtoFlux:HPReverbController#Usage)
  * [ 2 Examples ](https://wiki.resonite.com/ProtoFlux:HPReverbController#Examples)
  * [ 3 Inputs ](https://wiki.resonite.com/ProtoFlux:HPReverbController#Inputs)
    * [ 3.1 User (User) ](https://wiki.resonite.com/ProtoFlux:HPReverbController#User_\(User\))
    * [ 3.2 Node (Chirality) ](https://wiki.resonite.com/ProtoFlux:HPReverbController#Node_\(Chirality\))
  * [ 4 Outputs ](https://wiki.resonite.com/ProtoFlux:HPReverbController#Outputs)
    * [ 4.1 IsActive (bool) ](https://wiki.resonite.com/ProtoFlux:HPReverbController#IsActive_\(bool\))
    * [ 4.2 Type (Type) ](https://wiki.resonite.com/ProtoFlux:HPReverbController#Type_\(Type\))
    * [ 4.3 BatteryLevel (float) ](https://wiki.resonite.com/ProtoFlux:HPReverbController#BatteryLevel_\(float\))
    * [ 4.4 IsBatteryCharging (bool) ](https://wiki.resonite.com/ProtoFlux:HPReverbController#IsBatteryCharging_\(bool\))
    * [ 4.5 AppMenu (bool) ](https://wiki.resonite.com/ProtoFlux:HPReverbController#AppMenu_\(bool\))
    * [ 4.6 ButtonYB (bool) ](https://wiki.resonite.com/ProtoFlux:HPReverbController#ButtonYB_\(bool\))
    * [ 4.7 ButtonXA (bool) ](https://wiki.resonite.com/ProtoFlux:HPReverbController#ButtonXA_\(bool\))
    * [ 4.8 Grip (float) ](https://wiki.resonite.com/ProtoFlux:HPReverbController#Grip_\(float\))
    * [ 4.9 GripTouch (bool) ](https://wiki.resonite.com/ProtoFlux:HPReverbController#GripTouch_\(bool\))
    * [ 4.10 GripClick (bool) ](https://wiki.resonite.com/ProtoFlux:HPReverbController#GripClick_\(bool\))
    * [ 4.11 Joystick (float2) ](https://wiki.resonite.com/ProtoFlux:HPReverbController#Joystick_\(float2\))
    * [ 4.12 JoystickClick (bool) ](https://wiki.resonite.com/ProtoFlux:HPReverbController#JoystickClick_\(bool\))
    * [ 4.13 Trigger (float) ](https://wiki.resonite.com/ProtoFlux:HPReverbController#Trigger_\(float\))
    * [ 4.14 TriggerClick (bool) ](https://wiki.resonite.com/ProtoFlux:HPReverbController#TriggerClick_\(bool\))


[Categories](https://wiki.resonite.com/Special:Categories "Special:Categories"): 
  * [Stubs](https://wiki.resonite.com/Category:Stubs "Category:Stubs")
  * [ProtoFlux:All](https://wiki.resonite.com/Category:ProtoFlux:All "Category:ProtoFlux:All")
  * [ProtoFlux:Devices:Controllers](https://wiki.resonite.com/Category:ProtoFlux:Devices:Controllers "Category:ProtoFlux:Devices:Controllers")
  * [ContinuouslyChanging nodes](https://wiki.resonite.com/Category:ContinuouslyChanging_nodes "Category:ContinuouslyChanging nodes")


Last modified
This page was last edited on 21 August 2025, at 00:22.
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


