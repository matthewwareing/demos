# Blur Circles

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/blur-circles)
> **Source Code**: [/src/animations/blur-circles](/src/animations/blur-circles)

## Tags
- `skia`

## Description

Scan to try on your device

## Technical Implementation

- Perlin noise for natural movement
- Sweep gradients for color transitions
- Sophisticated blur masking
- Clip paths for complex visual effects
- Continuous animation using shared values

## Usage

```typescript
// The component is self-contained and can be used directly<BlurCircles />;
// Core animation configurationconst FREQUENCY = 0.8;const RADIUS = 45;const A = 60;
// Animation setupconst clock = useSharedValue(0);clock.value = withRepeat(  withTiming(20000, {    duration: 20000,  }),  -1,  true);
```

---

*Documentation extracted from reactiive.io/demos*
