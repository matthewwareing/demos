# Bezier Curve Outline

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/bezier-curve-outline)
> **Source Code**: [/src/animations/bezier-curve-outline](/src/animations/bezier-curve-outline)

## Tags
- `reanimated`
- `skia`
- `expo-blur`

## What's This About?

This component creates an interactive animation where a square moves along a Bézier curve path. When activated, it transitions into an outline mode with beautiful blur effects and color transitions. The animation includes smooth scaling and movement along the curve.

## Technical Implementation

The component leverages Skia for high-performance path rendering and Reanimated for fluid animations. It features:

- Smooth spring animations for transitions
- Path-based movement with progress tracking
- Dynamic blur intensity
- Color interpolation for status bar and text
- Gesture-based interactions

## Usage

```tsx
// The component is self-contained and can be used directly<BezierCurveOutline />;
// Core animation valuesconst outlineMode = useSharedValue(false);const blurIntensity = useSharedValue(0);const skiaPath = useSharedValue(Skia.Path.Make());
// Animation hook for path movementconst { progress, startAnimation, reverseAnimation } = useAnimateThroughPath({  pathReference: skiaPath,});
```

GitHubAsk for support

Bezier Curve Outline - FeedbackShare Your ThoughtsI value a lot your feedback! Help me improve by sharing your thoughts, suggestions, or reporting any issues you encounter. If you need assistance, send me an email at hello@reactiive.ioSend Feedback

---

*Documentation extracted from reactiive.io/demos*
