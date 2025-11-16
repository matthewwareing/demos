# Animated Count Text

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/animated-count-text)
> **Source Code**: [/src/animations/animated-count-text](/src/animations/animated-count-text)

## Tags
- `reanimated`

## What's This About?

This component animates number changes with a rolling animation effect. When the number updates, each digit smoothly transitions to its new value, creating a polished counting animation that's perfect for displaying dynamic numerical data.

## Technical Implementation

The component uses shared values and interpolated animations to handle individual digit transitions. It supports numbers of varying lengths and automatically adjusts its layout to accommodate different digit counts.

## Usage

```tsx
// Basic usage<AnimatedCount number={42} />;
// With dynamic updatesconst [number, setNumber] = useState(1);<AnimatedCount number={number} />;
```

GitHubAsk for support

Animated Count Text - FeedbackShare Your ThoughtsI value a lot your feedback! Help me improve by sharing your thoughts, suggestions, or reporting any issues you encounter. If you need assistance, send me an email at hello@reactiive.ioSend Feedback

---

*Documentation extracted from reactiive.io/demos*
