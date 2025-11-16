# Skia BottomSheet

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/skia-bottom-sheet)
> **Source Code**: [/src/animations/skia-bottom-sheet](/src/animations/skia-bottom-sheet)

## Tags
- `skia`

## Description

Scan to try on your device

## Technical Implementation

- Skia rendering
- Image handling
- Window sizing
- Touch gestures
- Responsive layout

## Usage

```typescript
// Basic usage<SkiaBottomSheet />
// Canvas setup with image<Touchable.Canvas  style={{ flex: 1 }}  onSize={size}>  <Image    x={0}    y={0}    width={imageWidth}    height={imageHeight}    fit="cover"    image={image}  />  <BottomSheet window={window} /></Touchable.Canvas>
// Window size handlingconst size = useSharedValue({ width: 0, height: 0 });const window = useDerivedValue(() => {  return {    width: size.value.width,    height: size.value.height  };}, [size]);
// Image dimensionsconst imageWidth = useDerivedValue(() => {  return window.value.width;}, [window]);
const imageHeight = useDerivedValue(() => {  return window.value.height;}, [window]);
```

---

*Documentation extracted from reactiive.io/demos*
