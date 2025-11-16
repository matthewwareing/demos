# Grid Visualizer

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/grid-visualizer)
> **Source Code**: [/src/animations/grid-visualizer](/src/animations/grid-visualizer)

## Tags
- `skia`

## What's This About?

This component creates an interactive visualization that displays numbers using a grid of animated squares. When tapped, it generates a random number and animates the grid to form that number's shape. The visualization includes a subtle radial gradient background and uses custom font rendering to create the number patterns, resulting in an engaging and modern display effect.

## Technical Implementation

The component uses:

- Skia for rendering
- Custom font loading
- Grid calculations
- Gesture handling
- Radial gradients

## Usage

```tsx
// Component propstype GridVisualizerProps = {  text: Animated.SharedValue<string | null>;  width: number;  height: number;  hSquaresAmount: number;  vSquaresAmount: number;  scaleFactor: number;  font: SkFont | null;  squareSize: number;};
// Basic usage<GridVisualizer  text={text}  width={300}  height={340}  hSquaresAmount={35}  vSquaresAmount={50}  scaleFactor={70}  font={font}  squareSize={2.5}/>;
```

GitHubAsk for support

Grid Visualizer - FeedbackShare Your ThoughtsI value a lot your feedback! Help me improve by sharing your thoughts, suggestions, or reporting any issues you encounter. If you need assistance, send me an email at hello@reactiive.ioSend Feedback

---

*Documentation extracted from reactiive.io/demos*
