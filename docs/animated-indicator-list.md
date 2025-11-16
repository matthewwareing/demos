# Animated Indicator List

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/animated-indicator-list)
> **Source Code**: [/src/animations/animated-indicator-list](/src/animations/animated-indicator-list)

## Tags
- `reanimated`
- `gesture-handler`

## What's This About?

This component implements a sectioned list with an animated indicator that follows the current section. As users scroll through the list or tap on section headers, the indicator smoothly animates to highlight the active section, providing clear visual feedback about the current position in the list.

## Technical Implementation

The component uses shared values to track scroll position and header layouts. It features precise measurements for header positioning, smooth animations for the indicator, and optimized scroll performance with event throttling.

## Usage

```tsx
type HeaderListItem = {  header: string;  type: 'header';};
type ListItem = {  id: string;  type: 'item';  title: string;};
// Example usage<AnimatedIndicatorList />;
```

GitHubAsk for support

Animated Indicator List - FeedbackShare Your ThoughtsI value a lot your feedback! Help me improve by sharing your thoughts, suggestions, or reporting any issues you encounter. If you need assistance, send me an email at hello@reactiive.ioSend Feedback

---

*Documentation extracted from reactiive.io/demos*
