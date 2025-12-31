# ProtoFlux:GetTexture3DPixel

> Source: https://wiki.resonite.com/ProtoFlux:GetTexture3DPixel

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
  * [English](https://wiki.resonite.com/ProtoFlux:GetTexture3DPixel)


Personal tools 
  * [](https://wiki.resonite.com/Special:MyTalk "Discussion about edits from this IP address \[n\]")
  * [](https://wiki.resonite.com/Special:MyContributions "A list of edits made from this IP address \[y\]")
  * [](https://wiki.resonite.com/index.php?title=Special:CreateAccount&returnto=ProtoFlux%3AGetTexture3DPixel "You are encouraged to create an account and log in; however, it is not mandatory")
  * [](https://wiki.resonite.com/index.php?title=Special:UserLogin&returnto=ProtoFlux%3AGetTexture3DPixel "You are encouraged to log in; however, it is not mandatory \[o\]")


#  ProtoFlux:GetTexture3DPixel
From Resonite Wiki
[](https://wiki.resonite.com/ProtoFlux:GetTexture3DPixel#top "Back to top \[home\]")
Views 
  * [](https://wiki.resonite.com/ProtoFlux:GetTexture3DPixel)
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:GetTexture3DPixel&action=edit "This page is protected.
You can view its source \[e\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:GetTexture3DPixel&action=history "Past revisions of this page \[h\]")


associated-pages 
  * [ProtoFlux](https://wiki.resonite.com/ProtoFlux:GetTexture3DPixel "View the subject page \[c\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux_talk:GetTexture3DPixel&action=edit&redlink=1 "Discussion about the content page \(page does not exist\) \[t\]")


More actions
More 
Tools 
  * [](https://wiki.resonite.com/Special:WhatLinksHere/ProtoFlux:GetTexture3DPixel "A list of all wiki pages that link here \[j\]")
  * [](https://wiki.resonite.com/Special:RecentChangesLinked/ProtoFlux:GetTexture3DPixel "Recent changes in pages linked from this page \[k\]")
  * [](javascript:print\(\); "Printable version of this page \[p\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:GetTexture3DPixel&oldid=113625 "Permanent link to this revision of this page")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:GetTexture3DPixel&action=info "More information about this page")


Get Texture 3D Pixel
Texture
*
Position
MipLevel
Assets
  
The **Get Texture 3D Pixel** node allows one to sample the pixel color of a [Texture3D](https://wiki.resonite.com/Texture3D "Texture3D") that has `Readable` enabled. Since the [StaticTexture3D](https://wiki.resonite.com/Component:StaticTexture3D "Component:StaticTexture3D") component needs to have `Readable` enabled, most players opt to keep a component on the object that their code is on, and then change it's URL so they can read the image's pixels. 
This node also takes a raw `IAsset[](https://wiki.resonite.com/Type:IAsset%601 "Type:IAsset`1")<Texture3D>` instead of an asset provider. To extract the raw texture reference from the provider for use in this node, see the [Get Asset](https://wiki.resonite.com/ProtoFlux:Get_Asset "ProtoFlux:Get Asset") node. 
## Inputs
### Texture ([IAsset](https://wiki.resonite.com/Type:IAsset%601 "Type:IAsset`1")<Texture3D>)
The raw asset of an [IAssetProvider<Texture3D>](https://wiki.resonite.com/Type:IAssetProvider%601 "Type:IAssetProvider`1") extracted using a [Get Asset Node](https://wiki.resonite.com/ProtoFlux:Get_Asset "ProtoFlux:Get Asset"). 
### Position ([Int3](https://wiki.resonite.com/Types:Int3 "Types:Int3"))
The Position to sample the colorX from. 
### MipLevel ([Int](https://wiki.resonite.com/Types:Int "Types:Int"))
The MipMap level of the provided image to sample from. Highest quality by default. 
## Outputs
### * ([colorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX"))
The ColorX color from the provided Texture ([IAsset](https://wiki.resonite.com/Type:IAsset%601 "Type:IAsset`1")<Texture3D>) at the provided Position ([Int3](https://wiki.resonite.com/Types:Int3 "Types:Int3")) with the provided quality MipLevel ([Int](https://wiki.resonite.com/Types:Int "Types:Int")). 
## Examples
  * [Example of a Get Texture3D Pixel being used in a larger example code reading 3D and 2D textures.](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=Protoflux_texture_asset_parsing.webp "File:Protoflux texture asset parsing.webp")
Example of a Get Texture3D Pixel being used in a larger example code reading 3D and 2D textures.


Retrieved from "[https://wiki.resonite.com/index.php?title=ProtoFlux:GetTexture3DPixel&oldid=113625](https://wiki.resonite.com/index.php?title=ProtoFlux:GetTexture3DPixel&oldid=113625)"
Contents [ Back to top ](https://wiki.resonite.com/ProtoFlux:GetTexture3DPixel#top "Back to top \[home\]")
Contents
  * [ 1 Inputs ](https://wiki.resonite.com/ProtoFlux:GetTexture3DPixel#Inputs)
    * [ 1.1 Texture (IAsset<Texture3D>) ](https://wiki.resonite.com/ProtoFlux:GetTexture3DPixel#Texture_\(IAsset<Texture3D>\))
    * [ 1.2 Position (Int3) ](https://wiki.resonite.com/ProtoFlux:GetTexture3DPixel#Position_\(Int3\))
    * [ 1.3 MipLevel (Int) ](https://wiki.resonite.com/ProtoFlux:GetTexture3DPixel#MipLevel_\(Int\))
  * [ 2 Outputs ](https://wiki.resonite.com/ProtoFlux:GetTexture3DPixel#Outputs)
    * [ 2.1 * (colorX) ](https://wiki.resonite.com/ProtoFlux:GetTexture3DPixel#*_\(colorX\))
  * [ 3 Examples ](https://wiki.resonite.com/ProtoFlux:GetTexture3DPixel#Examples)


[Categories](https://wiki.resonite.com/Special:Categories "Special:Categories"): 
  * [Pages with broken file links](https://wiki.resonite.com/Category:Pages_with_broken_file_links "Category:Pages with broken file links")
  * [ProtoFlux:All](https://wiki.resonite.com/Category:ProtoFlux:All "Category:ProtoFlux:All")
  * [ProtoFlux:Assets](https://wiki.resonite.com/Category:ProtoFlux:Assets "Category:ProtoFlux:Assets")


Last modified
This page was last edited on 19 October 2025, at 22:41.
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


