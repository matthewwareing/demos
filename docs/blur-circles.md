# Blur Circles

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/blur-circles)
> **Source Code**: [/src/animations/blur-circles](/src/animations/blur-circles)

## Tags
- `skia`

## What's This About?

This component creates an artistic visual effect where two circles interact: one with a colorful gradient and another with a glass-like blur effect. The circles move independently using different noise patterns, creating an engaging and organic animation.

## Technical Implementation

The component uses Skia for high-performance rendering and implements:

- Perlin noise for natural movement
- Sweep gradients for color transitions
- Sophisticated blur masking
- Clip paths for complex visual effects
- Continuous animation using shared values

## Usage

```tsx
// The component is self-contained and can be used directly<BlurCircles />;
// Core animation configurationconst FREQUENCY = 0.8;const RADIUS = 45;const A = 60;
// Animation setupconst clock = useSharedValue(0);clock.value = withRepeat(  withTiming(20000, {    duration: 20000,  }),  -1,  true);
```

GitHubAsk for support

Blur Circles - FeedbackShare Your ThoughtsI value a lot your feedback! Help me improve by sharing your thoughts, suggestions, or reporting any issues you encounter. If you need assistance, send me an email at hello@reactiive.ioSend Feedback

---

*Documentation extracted from reactiive.io/demos*
