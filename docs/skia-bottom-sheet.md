# Skia BottomSheet

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/skia-bottom-sheet)
> **Source Code**: [/src/animations/skia-bottom-sheet](/src/animations/skia-bottom-sheet)

## Tags
- `skia`

## What's This About?

This component creates a bottom sheet interface rendered entirely with Skia for optimal performance. It features a full-screen background image with a responsive bottom sheet overlay. The implementation handles window size changes and image fitting, making it suitable for applications requiring smooth interactions with visual content.

## Technical Implementation

The component uses:

- Skia rendering
- Image handling
- Window sizing
- Touch gestures
- Responsive layout

## Usage

```tsx
// Basic usage<SkiaBottomSheet />
// Canvas setup with image<Touchable.Canvas  style={{ flex: 1 }}  onSize={size}>  <Image    x={0}    y={0}    width={imageWidth}    height={imageHeight}    fit="cover"    image={image}  />  <BottomSheet window={window} /></Touchable.Canvas>
// Window size handlingconst size = useSharedValue({ width: 0, height: 0 });const window = useDerivedValue(() => {  return {    width: size.value.width,    height: size.value.height  };}, [size]);
// Image dimensionsconst imageWidth = useDerivedValue(() => {  return window.value.width;}, [window]);
const imageHeight = useDerivedValue(() => {  return window.value.height;}, [window]);
```

GitHubAsk for support

Skia Bottom Sheet - FeedbackShare Your ThoughtsI value a lot your feedback! Help me improve by sharing your thoughts, suggestions, or reporting any issues you encounter. If you need assistance, send me an email at hello@reactiive.ioSend Feedback

---

*Documentation extracted from reactiive.io/demos*
