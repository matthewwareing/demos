# Skia Color Picker

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/skia-color-picker)
> **Source Code**: [/src/animations/skia-color-picker](/src/animations/skia-color-picker)

## Tags
- `gesture-handler`
- `skia`

## What's This About?

This component creates an interactive color picker using Skia for optimal performance. It features a responsive canvas that adapts to the screen width, customizable blur effects, and real-time color updates. The implementation provides smooth color selection with gesture handling, making it suitable for applications requiring precise color picking capabilities.

## Technical Implementation

The component uses:

- Skia rendering
- Gesture handling
- Blur effects
- Color updates
- Screen adaptation

## Usage

```tsx
// Basic usage<SkiaColorPicker />
// Color picker with custom props<ColorPicker  canvasSize={windowWidth}  blur={20}  onColorUpdate={(color) => {    // Handle color updates    console.log(color);  }}/>
// With gesture handler root<GestureHandlerRootView style={{ flex: 1 }}>  <ColorPicker    canvasSize={windowWidth}    blur={20}    onColorUpdate={handleColorUpdate}  /></GestureHandlerRootView>
// Window dimensionsconst { width: canvasSize } = useWindowDimensions();
```

GitHubAsk for support

Skia Color Picker - FeedbackShare Your ThoughtsI value a lot your feedback! Help me improve by sharing your thoughts, suggestions, or reporting any issues you encounter. If you need assistance, send me an email at hello@reactiive.ioSend Feedback

---

*Documentation extracted from reactiive.io/demos*
