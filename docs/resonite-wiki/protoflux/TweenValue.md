# ProtoFlux:TweenValue

> Source: https://wiki.resonite.com/ProtoFlux:TweenValue

Tween

\*

OnStarted

To

OnDone

From

Duration

Curve

ProportionalDuration

Target

Actions

Tween Value is a node that allows you to change a Target ( [Numeric or Enum IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1")) over a Duration ( [float](https://wiki.resonite.com/Type:Float "Type:Float")) from a starting point to an ending point. The different curve presets determine the interpolation used, and when applicable will smoothly change using non whole numbers.

## Inputs

### \\* ( [AsyncCall](https://wiki.resonite.com/Impulses\#Async "Impulses"))

Tells the node to start tweening Target ( [Numeric or Enum IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1")).

### To (Pseudo-generic (Any Numeric or Enum value))

The value to tween towards over Duration ( [float](https://wiki.resonite.com/Type:Float "Type:Float"))

Examples: [Key Enum](https://wiki.resonite.com/Type:Key "Type:Key"), [Float](https://wiki.resonite.com/Type:Float "Type:Float"), [Int](https://wiki.resonite.com/Type:Int "Type:Int"), etc

### From (Pseudo-generic (Any Numeric or Enum value))

The value to tween away from over Duration ( [float](https://wiki.resonite.com/Type:Float "Type:Float"))

Examples: [Key Enum](https://wiki.resonite.com/Type:Key "Type:Key"), [Float](https://wiki.resonite.com/Type:Float "Type:Float"), [Int](https://wiki.resonite.com/Type:Int "Type:Int"), etc

### Duration ( [float](https://wiki.resonite.com/Type:Float "Type:Float"))

The duration in seconds that the value should tween for.

### Curve ( [CurvePreset](https://wiki.resonite.com/Type:CurvePreset "Type:CurvePreset"))

The interpolation type to use while tweening.

### ProportionalDuration ( [Boolean](https://wiki.resonite.com/Type:Bool "Type:Bool"))

If true, multiplies the duration of the tween by the distance between the two endpoints, making the average speed over the whole tween equal to 1.

### Target ( [Numeric or Enum IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1"))

The value this node should Tween.

## Outputs

### OnStarted ( [SyncResumption](https://wiki.resonite.com/Impulses\#Async "Impulses") (Async))

Sends an [Async Impulse](https://wiki.resonite.com/Impulses#Async "Impulses") once the node starts tweening the Target ( [Numeric or Enum IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1")).

### OnDone ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Sends an [Impulse](https://wiki.resonite.com/Impulses "Impulses") once the node is done tweening Target ( [Numeric or Enum IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1")).

## Examples

- [A short animation of a tween value moving something over time, with nodes beside it.](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=Protoflux_example_tween_value.gif "File:Protoflux example tween value.gif")

A short animation of a tween value moving something over time, with nodes beside it.


Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:TweenValue&oldid=113141](https://wiki.resonite.com/index.php?title=ProtoFlux:TweenValue&oldid=113141)"

Contents