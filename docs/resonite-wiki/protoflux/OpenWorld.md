# ProtoFlux:OpenWorld

> Source: https://wiki.resonite.com/ProtoFlux:OpenWorld

Open World

\*

OnOpenStart

URL

OnOpenDone

WorldLink

OnWorldReady

Relation

OnOpenFail

GetExisting

SessionID

LoadingIndicator

SessionURL

AutoFocus

MakePrivate

World

The `Open World` node is used to open a world when called, given a valid [Url](https://wiki.resonite.com/Type:Uri "Type:Uri") and a set of optional parameters the user can give it to open a world in a certain way. You can chain this node with the [Focus World](https://wiki.resonite.com/ProtoFlux:Focus_World "ProtoFlux:Focus World") node by using this node's SessionURL connected to the focus world node.

You can easily make a custom loading indicator using this node just by turning off the loading indicator and utilizing the OnOpenStart Async Continuation, however there is no way to make a custom loading bar to have an "accurate" percentage, thus is a tradeoff.

This node is also useful when making [Exit Strategies](https://wiki.resonite.com/Exit_Strategy "Exit Strategy"), as you can set it up to where if the world is valid to open and using the AutoFocus option, you can jump to the new focused world, and have the node continue from here to play a particle effect, a sound, and much more. Combining it further with the focus world node to close the old world is also an option.

## Inputs

### \\* ( [AsyncCall](https://wiki.resonite.com/Impulses "Impulses"))

Calls from an impulse to open a world with a given URL.

### URL ( [Uri](https://wiki.resonite.com/Type:Uri "Type:Uri"))

The World URL needed to open a world.

### WorldLink ( [IWorldLink](https://wiki.resonite.com/index.php?title=Type:IWorldLink&action=edit&redlink=1 "Type:IWorldLink (page does not exist)"))

The link to a world (using the [WorldLink](https://wiki.resonite.com/Component:WorldLink "Component:WorldLink") component). This can be an alternative way of opening a world.

### Relation ( [Relation](https://wiki.resonite.com/Type:Relation "Type:Relation"))

The relation to a world (Not necessary for opening a world). See the Relation Type for more info.

### GetExisting ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Should this try to get an already opened world first.

### LoadingIndicator ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Should this show a loading indicator to the user that is opening the world.

### AutoFocus ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Should this automatically focus the user to the opened world as soon as it opens.

### MakePrivate ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Should this make the opening world private when opening it.

## Outputs

### OnOpenStart ( [AsyncCall](https://wiki.resonite.com/Impulses "Impulses"))

Fires when the world has started to open.

### OnOpenDone ( [AsyncCall](https://wiki.resonite.com/Impulses "Impulses"))

Fires when the world has finished opening.

### OnWorldReady ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Fires when the world has finished opening and is ready to hold users.

### OnOpenFail ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Fires when the world could not be opened or the world URL is not valid.

### SessionID ( [String](https://wiki.resonite.com/Type:String "Type:String"))

The session ID for the opened world and user connection to it.

### SessionURL ( [Uri](https://wiki.resonite.com/Type:Uri "Type:Uri"))

The world URL for the opened session.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:OpenWorld&oldid=110381](https://wiki.resonite.com/index.php?title=ProtoFlux:OpenWorld&oldid=110381)"

Contents