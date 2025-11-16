# Infinite Carousel

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/infinite-carousel)
> **Source Code**: [/src/animations/infinite-carousel](/src/animations/infinite-carousel)

## Tags
- `reanimated`
- `gesture-handler`

## Description

Scan to try on your device

## Technical Implementation

- Circular scrolling logic
- Dynamic theming
- Custom interpolation
- Gradient backgrounds
- Item animations

## Usage

```typescript
// Basic usage with configuration<InfiniteCircularCarousel  ref={carouselRef}  data={ThemeData}  listItemWidth={ListItemSize}  centered  snapEnabled  onActiveIndexChanged={(index) => {    // Handle index change  }}  interpolateConfig={{    inputRange: (index) => [      (index - 2) * ListItemSize,      (index - 1) * ListItemSize,      index * ListItemSize,      (index + 1) * ListItemSize,      (index + 2) * ListItemSize,    ],    outputRange: () => [-1, -1.5, 0, 1.5, 1],    extrapolationType: Extrapolation.CLAMP,  }}  renderItem={({ item, index, progress }) => (    <ListItemCard      item={item}      index={index}      progress={progress}      onPress={() => {        carouselRef.current?.scrollToIndex(index);      }}    />  )}/>
```

---

*Documentation extracted from reactiive.io/demos*
