# Alert Drawer

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/alert-drawer)
> **Source Code**: [/src/animations/alert-drawer](/src/animations/alert-drawer)

## Tags
- `reanimated`

## What's This About?

This component transforms between two states: a compact button and an expanded alert card. When activated, it smoothly animates to reveal additional information, action buttons, and a close option, creating a seamless transition that maintains context.

## Technical Implementation

The component uses interpolated animations for size, color, and position transitions. It features precise timing controls and smooth state management to ensure fluid transformations between the button and expanded states.

## Usage

```tsx
type AlertDrawerProps = {  title: string;  description: string;  buttonLabel: string;  onConfirm?: () => void;};
// Example usage<AlertDrawer  title="Are you sure?"  description="Confirmation message here"  buttonLabel="Continue"  onConfirm={() => console.log('Confirmed')}/>;
```

GitHubAsk for support

Alert Drawer - FeedbackShare Your ThoughtsI value a lot your feedback! Help me improve by sharing your thoughts, suggestions, or reporting any issues you encounter. If you need assistance, send me an email at hello@reactiive.ioSend Feedback

---

*Documentation extracted from reactiive.io/demos*
