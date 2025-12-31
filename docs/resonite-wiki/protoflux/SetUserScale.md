# ProtoFlux:SetUserScale

> Source: https://wiki.resonite.com/ProtoFlux:SetUserScale

Set User Scale

\*

OnScaleChangeStart

UserRoot

OnAnimationFinished

Scale

AnimationTime

Users

The `Set User Scale` node changes the user scale with the provided inputs. While the user is scaling and the user is in the middle of a scale animation, the user cannot be scaled again until the animation has finished.

![](https://wiki.resonite.com/images/d/dd/InformationIcon.svg)

There is a set of features in [Resonite](https://wiki.resonite.com/Resonite "Resonite") that allows you to [scale and calculate scale](https://wiki.resonite.com/User_Scale "User Scale") in different ways.


## Inputs

### \\* ( [AsyncCall](https://wiki.resonite.com/Impulses "Impulses"))

Calls from an impulse to start changing the user's scale.

### UserRoot ( [UserRoot](https://wiki.resonite.com/Type:UserRoot "Type:UserRoot"))

The user root to scale.

### Scale ( [float](https://wiki.resonite.com/Type:Float "Type:Float"))

The target scale to aim for.

### AnimationTime ( [float](https://wiki.resonite.com/Type:Float "Type:Float"))

How long this scaling should take.

## Outputs

### OnScaleChangeStart ( [AsyncCall](https://wiki.resonite.com/Impulses "Impulses"))

Fires when the scaling has started.

### OnAnimationFinished ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Fires when the scaling animation has finished scaling the user.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:SetUserScale&oldid=110737](https://wiki.resonite.com/index.php?title=ProtoFlux:SetUserScale&oldid=110737)"

Contents