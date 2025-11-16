# Color Carousel

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/color-carousel)
> **Source Code**: [/src/animations/color-carousel](/src/animations/color-carousel)

## Tags
- `reanimated`
- `skia`

## Description

Scan to try on your device

## Technical Implementation

- Smooth carousel transitions
- Dynamic radial gradient backgrounds
- Configurable number of visible items
- Optimized rendering with a fixed number of items
- Shared value animations for color transitions

## Usage

```typescript
type CarouselItem = {  accentColor: string;  // other item properties};
// Basic usage<ColorCarousel />
// Custom implementation<Carousel  items={data}  maxRenderedItems={5}  // Must be an odd number  width={windowWidth}  activeIndex={activeIndex}/>
// With background gradient<Canvas style={StyleSheet.absoluteFill}>  <Rect x={0} y={0} width={width} height={height}>    <RadialGradient      c={vec(width/2, height/2)}      r={width/2}      colors={colors}    />  </Rect></Canvas>
```

---

*Documentation extracted from reactiive.io/demos*
