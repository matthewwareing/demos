# Fluid Slider

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/fluid-slider)
> **Source Code**: [/src/animations/fluid-slider](/src/animations/fluid-slider)

## Tags
- `gesture-handler`
- `skia`

## What's This About?

This component implements a modern slider control that features fluid animations through metaball effects. As users interact with the slider, a dynamic bubble follows the touch point, displaying the current value. The slider adapts to different screen sizes while maintaining smooth animations and precise touch handling.

## Technical Implementation

The component uses:

- Skia for metaball effects
- Responsive sizing
- Gesture handling
- Value interpolation
- Window dimensions

## Usage

```tsx
type FluidSliderProps = {  width: number;  height: number;};
// Basic usageconst { width } = useWindowDimensions();
<FluidSlider width={width * 0.9} height={110} />;// Note: Height should account for the// animated metaball with text
```

GitHubAsk for support

Fluid Slider - FeedbackShare Your ThoughtsI value a lot your feedback! Help me improve by sharing your thoughts, suggestions, or reporting any issues you encounter. If you need assistance, send me an email at hello@reactiive.ioSend Feedback

---

*Documentation extracted from reactiive.io/demos*
