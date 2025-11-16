# Fibonacci Shader

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/fibonacci-shader)
> **Source Code**: [/src/animations/fibonacci-shader](/src/animations/fibonacci-shader)

## Tags
- `reanimated`
- `skia`

## Description

Scan to try on your device

## What's This About?

- Generates circular patterns
- Allows pattern customization
- Uses performance scaling
- Supports interactive controls
- Animates continuously

## Technical Implementation

- Skia for shader rendering
- Runtime shader compilation
- Performance optimization
- Reanimated for timing
- Dynamic uniforms

## Usage

```typescript
// Basic usage<FibonacciShader />;
// Component parametersconst RESCALE_FACTOR = 4; // Performance vs qualityconst MAX_CIRCLES_AMOUNT = 350; // Maximum circles to render
// Shader controlsconst N = useSharedValue(5.0); // Number of circlesconst magicalMul = useSharedValue(2.4); // Pattern multiplier
// Animation timingiTime.value = withRepeat(  withTiming(15, {    duration: 20000,    easing: Easing.linear,  }),  -1,  true);
```

---

*Documentation extracted from reactiive.io/demos*
