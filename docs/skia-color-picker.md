# Skia Color Picker

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/skia-color-picker)
> **Source Code**: [/src/animations/skia-color-picker](/src/animations/skia-color-picker)

## Tags
- `gesture-handler`
- `skia`

## Description

Scan to try on your device

## Technical Implementation

- Skia rendering
- Gesture handling
- Blur effects
- Color updates
- Screen adaptation

## Usage

```typescript
// Basic usage<SkiaColorPicker />
// Color picker with custom props<ColorPicker  canvasSize={windowWidth}  blur={20}  onColorUpdate={(color) => {    // Handle color updates    console.log(color);  }}/>
// With gesture handler root<GestureHandlerRootView style={{ flex: 1 }}>  <ColorPicker    canvasSize={windowWidth}    blur={20}    onColorUpdate={handleColorUpdate}  /></GestureHandlerRootView>
// Window dimensionsconst { width: canvasSize } = useWindowDimensions();
```

---

*Documentation extracted from reactiive.io/demos*
