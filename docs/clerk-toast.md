# Clerk Toast

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/clerk-toast)
> **Source Code**: [/src/animations/clerk-toast](/src/animations/clerk-toast)

## Tags
- `reanimated`

## Description

Scan to try on your device

## Technical Implementation

- Stacked notification management
- Gesture-based interactions
- Smooth enter/exit animations
- Safe area handling
- Automatic toast queuing
- Scale animations on press
- Custom styling options

## Usage

```typescript
// Setup the provider<StackedToastProvider>  <App /></StackedToastProvider>;
// Using the toast hookconst { showToast } = useStackedToast();
// Show a toastshowToast({  title: 'Notification Title',  message: 'Your notification message here',});
```

---

*Documentation extracted from reactiive.io/demos*
