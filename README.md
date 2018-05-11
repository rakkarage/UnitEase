# UnitEase: Unity Bolt Easing

rakkarage@gmail.com

Based on:

- http://robertpenner.com/easing/
- https://github.com/rakkarage/Ease
- many other easing systems


## Instructions

You can drag a Flow Macro into your flow and hook it up like I do in intro.
It takes an ease type, a from and to value, a time, and it outputs the value beTWEEN from and to for the given time.

Or you can attach a Flow State and set variables.

TODO:

- mostly broken garbage but intro example works well
- need to make GoAlpha etc work
- need to make multiple work on same object with diff variables? no way to pass into a state?

### Flow States

- GoAlpha
- GoAlphaBy
- GoAlphaTo
- GoColor
- GoColorBy
- GoColorTo
- GoPosition
- GoPositionBy
- GoPositionTo
- GoRotation
- GoRotationBy
- GoRotationTo
- GoScale
- GoScaleBy
- GoScaleTo

### Flow Macros

- UnitEase
- UnitEase2
- UnitEase3
- UnitEase4

### Type Flow Macros

- Linear,
- SineIn, SineOut, SineInOut,
- QuadIn, QuadOut, QuadInOut,
- CubicIn, CubicOut, CubicInOut,
- QuartIn, QuartOut, QuartInOut,
- QuintIn, QuintOut, QuintInOut,
- xpoIn, ExpoOut, ExpoInOut,
- CircIn, CircOut, CircInOut,
- BackIn, BackOut, BackInOut,
- ElasticIn, ElasticOut, ElasticInOut,
- BounceIn, BounceOut, BounceInOut,
- Spring

### Input Variables

- type: EaseType
    - default: linear
- from: float, vector2, 3, 4
    - default: 0, (0, 0), (0, 0, 0), (0, 0, 0, 0)
- to: float
    - default: 1, (1, 1), (1, 1, 1), (1, 1, 1, 1)
- time: float
    - default: 1, (1, 1), (1, 1, 1), (1, 1, 1, 1)
- delay: float
    - default: 0, (0, 0), (0, 0, 0), (0, 0, 0, 0)
- unscaled: bool (use unscaled time, for ui)
    - default: false
- repeat: int (0 or -1 = forever)
    - default: 1
- pingPong: bool (each repeat includes reverse back to start?)
    - default: false
