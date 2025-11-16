# Paper Folding

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/paper-folding)
> **Source Code**: [/src/animations/paper-folding](/src/animations/paper-folding)

## Tags
- `skia`

## What's This About?

This component creates an interactive paper folding animation that responds to touch events. When touched, a paper-like element smoothly transitions between folded and unfolded states, creating a realistic folding effect. The component includes a gradient background that enhances the visual depth of the animation, making the paper appear to float above the surface.

## Technical Implementation

The component uses:

- Touch handling
- Timing animations
- Gradient backgrounds
- Paper folding effects
- Dimension control

## Usage

```tsx
// Basic usage<PaperFolding />;
// Component configurationconst PaperWidth = 250;const PaperHeight = 330;
// Animation controlconst progress = useSharedValue(0);
// Paper component with props<Paper width={PaperWidth} height={PaperHeight} progress={progress} />;
// Animation triggerprogress.value = withTiming(progress.value > 0 ? 0 : 1, {  duration: 800,});
```

GitHubAsk for support

Paper Folding - FeedbackShare Your ThoughtsI value a lot your feedback! Help me improve by sharing your thoughts, suggestions, or reporting any issues you encounter. If you need assistance, send me an email at hello@reactiive.ioSend Feedback

---

*Documentation extracted from reactiive.io/demos*
