# Fibonacci Shader Grid

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/fibonacci-shader-grid)
> **Source Code**: [/src/animations/fibonacci-shader-grid](/src/animations/fibonacci-shader-grid)

## Tags
- `reanimated`
- `gesture-handler`
- `skia`

## Description

Scan to try on your device

## What's This About?

- Shows multiple pattern instances
- Provides control panel
- Allows pattern adjustment
- Handles performance scaling
- Supports value constraints

## Technical Implementation

- Skia shader rendering
- Control panel interface
- Value range management
- Performance optimization
- Dynamic shader updates

## Usage

```typescript
// Basic usage<FibonacciShaderGrid />;
// Configuration constantsconst RESCALE_FACTOR = 3;const MIN_CIRCLES_AMOUNT = 5;const MAX_CIRCLES_AMOUNT = 175;const MIN_MAGICAL_MUL = 1.2;const MAX_MAGICAL_MUL = 3.6;
// Control valuesconst n = useSharedValue(INITIAL_CIRCLES_AMOUNT);const magicalMul = useSharedValue(INITIAL_MAGICAL_MUL);
// Control panel<ControlPanel  n={n}  magicalMul={magicalMul}  minN={MIN_CIRCLES_AMOUNT}  maxN={MAX_CIRCLES_AMOUNT}  minMagicalMul={MIN_MAGICAL_MUL}  maxMagicalMul={MAX_MAGICAL_MUL}/>;
```

---

*Documentation extracted from reactiive.io/demos*
