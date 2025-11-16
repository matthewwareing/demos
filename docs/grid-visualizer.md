# Grid Visualizer

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/grid-visualizer)
> **Source Code**: [/src/animations/grid-visualizer](/src/animations/grid-visualizer)

## Tags
- `skia`

## Description

Scan to try on your device

## Technical Implementation

- Skia for rendering
- Custom font loading
- Grid calculations
- Gesture handling
- Radial gradients

## Usage

```typescript
// Component propstype GridVisualizerProps = {  text: Animated.SharedValue<string | null>;  width: number;  height: number;  hSquaresAmount: number;  vSquaresAmount: number;  scaleFactor: number;  font: SkFont | null;  squareSize: number;};
// Basic usage<GridVisualizer  text={text}  width={300}  height={340}  hSquaresAmount={35}  vSquaresAmount={50}  scaleFactor={70}  font={font}  squareSize={2.5}/>;
```

---

*Documentation extracted from reactiive.io/demos*
