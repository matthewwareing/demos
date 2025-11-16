# Fibonacci Shader

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/fibonacci-shader)
> **Source Code**: [/src/animations/fibonacci-shader](/src/animations/fibonacci-shader)

## Tags
- `reanimated`
- `skia`

## What's This About?

Fibonacci Shader - FeedbackShare Your ThoughtsI value a lot your feedback! Help me improve by sharing your thoughts, suggestions, or reporting any issues you encounter. If you need assistance, send me an email at hello@reactiive.ioSend Feedback

## Technical Implementation

The component uses:

- Skia for shader rendering
- Runtime shader compilation
- Performance optimization
- Reanimated for timing
- Dynamic uniforms

## Usage

```tsx
// Basic usage<FibonacciShader />;
// Component parametersconst RESCALE_FACTOR = 4; // Performance vs qualityconst MAX_CIRCLES_AMOUNT = 350; // Maximum circles to render
// Shader controlsconst N = useSharedValue(5.0); // Number of circlesconst magicalMul = useSharedValue(2.4); // Pattern multiplier
// Animation timingiTime.value = withRepeat(  withTiming(15, {    duration: 20000,    easing: Easing.linear,  }),  -1,  true);
```

GitHubAsk for support

Fibonacci Shader - FeedbackShare Your ThoughtsI value a lot your feedback! Help me improve by sharing your thoughts, suggestions, or reporting any issues you encounter. If you need assistance, send me an email at hello@reactiive.ioSend Feedback

---

*Documentation extracted from reactiive.io/demos*
