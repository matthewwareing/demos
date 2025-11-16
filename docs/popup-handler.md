# Popup Handler

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/popup-handler)
> **Source Code**: [/src/animations/popup-handler](/src/animations/popup-handler)

## Tags
- `gesture-handler`
- `skia`

## What's This About?

This component creates an interactive popup interface that can be dragged around the screen and snaps to different corners. It features a blurred background effect and supports various positioning options (top-left, top-right, bottom-left, bottom-right). The popup includes rotation animations based on its position and gesture handling for smooth dragging interactions.

## Technical Implementation

The component uses:

- Gesture handling
- Position snapping
- Blurred backgrounds
- Corner rotation
- Spring animations

## Usage

```tsx
// Basic usage<PopupHandler />;
// Popup configurationtype Angle = 'top-left' | 'top-right' | 'bottom-left' | 'bottom-right';
// Gesture setupconst gesture = Gesture.Pan()  .onBegin(() => {    context.value = {      x: translateX.value,      y: translateY.value,    };  })  .onUpdate((event) => {    translateX.value = event.translationX + context.value.x;    translateY.value = event.translationY + context.value.y;  });
// With blurred background<BlurredPopupProvider>  <TouchablePopupHandler>{/* Popup content */}</TouchablePopupHandler></BlurredPopupProvider>;
```

GitHubAsk for support

Popup Handler - FeedbackShare Your ThoughtsI value a lot your feedback! Help me improve by sharing your thoughts, suggestions, or reporting any issues you encounter. If you need assistance, send me an email at hello@reactiive.ioSend Feedback

---

*Documentation extracted from reactiive.io/demos*
