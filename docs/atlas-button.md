# Atlas Button

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/atlas-button)
> **Source Code**: [/src/animations/atlas-button](/src/animations/atlas-button)

## Tags
- `skia`

## What's This About?

This component creates a button with a dynamic grid of colored squares that respond to interaction. The squares use a carefully selected color palette with varying probabilities, creating a visually appealing pattern that enhances the button's appearance.

## Technical Implementation

The component uses Skia for high-performance rendering of the color squares. It implements a sophisticated color distribution system using Float32Arrays and supports custom SVG icons and labels.

## Usage

```tsx
type AtlasButtonProps = {  width: number;  height: number;  label: string;  svgIcon: any;  colors: Float32Array[];  horizontalSquaresAmount: number;  onPress: () => void;};
// Example usage<AtlasButton  width={250}  height={200}  label="React Native"  svgIcon={YourSvgIcon}  colors={colors}  horizontalSquaresAmount={50}  onPress={() => {}}/>;
```

GitHubAsk for support

Atlas Button - FeedbackShare Your ThoughtsI value a lot your feedback! Help me improve by sharing your thoughts, suggestions, or reporting any issues you encounter. If you need assistance, send me an email at hello@reactiive.ioSend Feedback

---

*Documentation extracted from reactiive.io/demos*
