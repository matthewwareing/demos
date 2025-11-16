# Fluid Slider

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/fluid-slider)
> **Source Code**: [/src/animations/fluid-slider](/src/animations/fluid-slider)

## Tags
- `gesture-handler`
- `skia`

## Description

Scan to try on your device

## Technical Implementation

- Skia for metaball effects
- Responsive sizing
- Gesture handling
- Value interpolation
- Window dimensions

## Usage

```typescript
type FluidSliderProps = {  width: number;  height: number;};
// Basic usageconst { width } = useWindowDimensions();
<FluidSlider width={width * 0.9} height={110} />;// Note: Height should account for the// animated metaball with text
```

---

*Documentation extracted from reactiive.io/demos*
