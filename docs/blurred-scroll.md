# Blurred Scroll

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/blurred-scroll)
> **Source Code**: [/src/animations/blurred-scroll](/src/animations/blurred-scroll)

## Tags
- `reanimated`
- `skia`

## Description

Scan to try on your device

## Technical Implementation

- Dynamic blur effects based on scroll position
- Optimized scroll performance with event throttling
- Pre-calculated item layouts for smooth scrolling
- Responsive sizing based on window dimensions
- Fade-in animations for items

## Usage

```typescript
// Core animation setupconst contentOffsetY = useSharedValue(0);const scrollHandler = useAnimatedScrollHandler({  onScroll: (event) => {    contentOffsetY.value = event.contentOffset.y;  },});
// Item configuration<BlurredItem  width={windowWidth}  height={blurredItemContainerHeight}  index={index}  contentOffsetY={contentOffsetY}/>;
```

---

*Documentation extracted from reactiive.io/demos*
