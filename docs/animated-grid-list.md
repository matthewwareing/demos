# Animated Grid List

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/animated-grid-list)
> **Source Code**: [/src/animations/animated-grid-list](/src/animations/animated-grid-list)

## Tags
- `reanimated`

## What's This About?

This component provides a seamless way to display content in both grid and list views. Users can toggle between layouts with a floating button, and the content smoothly animates between states. Images resize and reposition while text fades in and out appropriately.

## Technical Implementation

The component uses layout animations for smooth transitions and handles image aspect ratios dynamically. It features fade animations for text content and supports custom rendering of items in both layouts.

## Usage

```tsx
type Item = {  img: string;  title: string;  subtitle: string;};
// Example usage<AnimatedLayoutList  data={items}  layout="grid"  renderItem={(item, index, isExpanded) => (    // Custom render implementation  )}/>
```

GitHubAsk for support

Animated Grid List - FeedbackShare Your ThoughtsI value a lot your feedback! Help me improve by sharing your thoughts, suggestions, or reporting any issues you encounter. If you need assistance, send me an email at hello@reactiive.ioSend Feedback

---

*Documentation extracted from reactiive.io/demos*
