# Bezier Curve Outline

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/bezier-curve-outline)
> **Source Code**: [/src/animations/bezier-curve-outline](/src/animations/bezier-curve-outline)

## Tags
- `reanimated`
- `skia`
- `expo-blur`

## Description

Scan to try on your device

## Technical Implementation

- Smooth spring animations for transitions
- Path-based movement with progress tracking
- Dynamic blur intensity
- Color interpolation for status bar and text
- Gesture-based interactions

## Usage

```typescript
// The component is self-contained and can be used directly<BezierCurveOutline />;
// Core animation valuesconst outlineMode = useSharedValue(false);const blurIntensity = useSharedValue(0);const skiaPath = useSharedValue(Skia.Path.Make());
// Animation hook for path movementconst { progress, startAnimation, reverseAnimation } = useAnimateThroughPath({  pathReference: skiaPath,});
```

---

*Documentation extracted from reactiive.io/demos*
