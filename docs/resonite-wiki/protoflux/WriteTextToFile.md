# ProtoFlux:WriteTextToFile

> Source: https://wiki.resonite.com/ProtoFlux:WriteTextToFile

Write Text To File

\*

OnWriteStarted

String

OnWriteFinished

FilePath

OnWriteFail

Append

NewLine

Experimental

The `Write Text To File` node allows you to write files to your device, given if there is a path and proper permissions.

Currently at this time, this node is experimental, and thus cannot be used normally without making the world private, setting it to unsafe mode, and then running the node. Please note that making the world in unsafe mode does not allow other users to join under any circumstances.

## Inputs

### \\* ( [IAsyncOperation](https://wiki.resonite.com/Impulses "Impulses"))

Calls from an impulse to write a file on the user's computer.

### String ( [String](https://wiki.resonite.com/Type:String "Type:String"))

The contents for this file.

### FilePath ( [String](https://wiki.resonite.com/Type:String "Type:String"))

The path where the file should be saved/written to.

### Append ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Should add on to the file when writting to it.

### NewLine ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Should make a new line when adding to this file.

## Outputs

### OnWriteStarted ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Fires when the file writing process has started.

### OnWriteFinished ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Fires when the file is written successfully.

### OnWriteFail ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Fires when there is no file to write to or the user did not give/have permission to write a file there.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:WriteTextToFile&oldid=111173](https://wiki.resonite.com/index.php?title=ProtoFlux:WriteTextToFile&oldid=111173)"

Contents