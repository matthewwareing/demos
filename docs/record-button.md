# Record Button

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/record-button)
> **Source Code**: [/src/animations/record-button](/src/animations/record-button)

## Tags
- `skia`

## Description

Scan to try on your device

## Technical Implementation

- Scroll offset tracking
- Interpolated animations
- Snapping behavior
- Border radius transitions
- Custom button styling

## Usage

```typescript
// Basic usage<RecordButton />;
// Button configurationconst ButtonConfig = {  width: 90,  height: 40,  radius: 20,  strokeWidth: 1,  color: '#ed4e3c',};
// Scroll interpolationconst progress = useDerivedValue(() => {  return interpolate(    scrollOffset.value,    [WindowHeight * 0.08, WindowHeight * 0.2],    [0, 1],    Extrapolation.CLAMP  );});
// Border radius animationconst rMainPageStyle = useAnimatedStyle(() => {  return {    borderCurve: 'continuous',    borderRadius: interpolate(      scrollOffset.value,      [0, 0.1],      [0, 35],      Extrapolation.CLAMP    ),  };});
```

---

*Documentation extracted from reactiive.io/demos*
