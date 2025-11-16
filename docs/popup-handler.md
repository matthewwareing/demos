# Popup Handler

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/popup-handler)
> **Source Code**: [/src/animations/popup-handler](/src/animations/popup-handler)

## Tags
- `gesture-handler`
- `skia`

## Description

Scan to try on your device

## Technical Implementation

- Gesture handling
- Position snapping
- Blurred backgrounds
- Corner rotation
- Spring animations

## Usage

```typescript
// Basic usage<PopupHandler />;
// Popup configurationtype Angle = 'top-left' | 'top-right' | 'bottom-left' | 'bottom-right';
// Gesture setupconst gesture = Gesture.Pan()  .onBegin(() => {    context.value = {      x: translateX.value,      y: translateY.value,    };  })  .onUpdate((event) => {    translateX.value = event.translationX + context.value.x;    translateY.value = event.translationY + context.value.y;  });
// With blurred background<BlurredPopupProvider>  <TouchablePopupHandler>{/* Popup content */}</TouchablePopupHandler></BlurredPopupProvider>;
```

---

*Documentation extracted from reactiive.io/demos*
