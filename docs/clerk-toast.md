# Clerk Toast

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/clerk-toast)
> **Source Code**: [/src/animations/clerk-toast](/src/animations/clerk-toast)

## Tags
- `reanimated`

## What's This About?

This component implements a stacked toast notification system where multiple notifications can be displayed simultaneously. Each toast can be interacted with through gestures, and the stack automatically manages the layout and animations of multiple notifications.

## Technical Implementation

The component implements:

- Stacked notification management
- Gesture-based interactions
- Smooth enter/exit animations
- Safe area handling
- Automatic toast queuing
- Scale animations on press
- Custom styling options

## Usage

```tsx
// Setup the provider<StackedToastProvider>  <App /></StackedToastProvider>;
// Using the toast hookconst { showToast } = useStackedToast();
// Show a toastshowToast({  title: 'Notification Title',  message: 'Your notification message here',});
```

GitHubAsk for support

Clerk Toast - FeedbackShare Your ThoughtsI value a lot your feedback! Help me improve by sharing your thoughts, suggestions, or reporting any issues you encounter. If you need assistance, send me an email at hello@reactiive.ioSend Feedback

---

*Documentation extracted from reactiive.io/demos*
