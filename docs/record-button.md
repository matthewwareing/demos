# Record Button

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/record-button)
> **Source Code**: [/src/animations/record-button](/src/animations/record-button)

## Tags
- `skia`

## What's This About?

This component creates an interactive record button interface with sophisticated scroll animations. As users scroll, the interface smoothly transitions between states, featuring border radius animations and a custom record button. The implementation includes scroll-based interpolation, snapping behavior, and precise animation timing, making it suitable for media recording applications.

## Technical Implementation

The component uses:

- Scroll offset tracking
- Interpolated animations
- Snapping behavior
- Border radius transitions
- Custom button styling

## Usage

```tsx
// Basic usage<RecordButton />;
// Button configurationconst ButtonConfig = {  width: 90,  height: 40,  radius: 20,  strokeWidth: 1,  color: '#ed4e3c',};
// Scroll interpolationconst progress = useDerivedValue(() => {  return interpolate(    scrollOffset.value,    [WindowHeight * 0.08, WindowHeight * 0.2],    [0, 1],    Extrapolation.CLAMP  );});
// Border radius animationconst rMainPageStyle = useAnimatedStyle(() => {  return {    borderCurve: 'continuous',    borderRadius: interpolate(      scrollOffset.value,      [0, 0.1],      [0, 35],      Extrapolation.CLAMP    ),  };});
```

GitHubAsk for support

Record Button - FeedbackShare Your ThoughtsI value a lot your feedback! Help me improve by sharing your thoughts, suggestions, or reporting any issues you encounter. If you need assistance, send me an email at hello@reactiive.ioSend Feedback

---

*Documentation extracted from reactiive.io/demos*
