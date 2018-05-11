# UnitEase: Unity Bolt Easing

rakkarage@gmail.com

Based on:

- http://robertpenner.com/easing/
- https://github.com/rakkarage/Ease
- many other easing systems


## Instructions

You can drag a Flow Macro into your flow and hook it up like I do in intro.
It takes an ease type, a from and to value, a time, and it outputs the value beTWEEN from and to.

Or you can attach a Flow State and set variables.

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
- from: float
- to: float
- time: float
- delay: float
- unscaled: bool (use unscaled time, for ui)
- repeat: int (0 or -1 = forever)
- pingPong: bool (each repeat includes reverse back to start?)
