# Animated Clip Box

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/animated-clip-box)
> **Source Code**: [/src/animations/animated-clip-box](/src/animations/animated-clip-box)

## Tags
- `reanimated`
- `skia`

## What's This About?

This component creates an interactive button that responds to touch with a smooth expanding circle animation. The circle clips the content and changes text colors dynamically, creating a fluid transition between states. When pressed, the circle expands to fill the entire button while smoothly transitioning text colors.

## Technical Implementation

The component uses spring animations and color interpolation for smooth transitions. It features precise clipping calculations and touch handling to ensure the expanding circle animation feels natural and responsive.

## Usage

```tsx
type ClipBoxButtonProps = {  style: StyleProp<ViewStyle>;  initialRadius?: number;  primaryColor?: string;  highlightColor?: string;  description: string;  actionTitle: string;  onPress?: () => void;};
// Example usage<ClipBoxButton  description="Button description here"  actionTitle="Click Me"  primaryColor="#4BA2E4"  highlightColor="#83C5F1"/>;
```

GitHubAsk for support

Animated Clip Box - FeedbackShare Your ThoughtsI value a lot your feedback! Help me improve by sharing your thoughts, suggestions, or reporting any issues you encounter. If you need assistance, send me an email at hello@reactiive.ioSend Feedback

---

*Documentation extracted from reactiive.io/demos*
