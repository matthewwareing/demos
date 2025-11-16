# Infinite Carousel

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/infinite-carousel)
> **Source Code**: [/src/animations/infinite-carousel](/src/animations/infinite-carousel)

## Tags
- `reanimated`
- `gesture-handler`

## What's This About?

This component creates an advanced carousel that provides seamless infinite scrolling in both directions. It features dynamic theme transitions, where the background color smoothly changes based on the active item. The carousel supports custom item rendering, precise snap behavior, and configurable interpolation for item animations. The implementation includes optimizations for smooth performance and a visually appealing interface with gradient backgrounds.

## Technical Implementation

The component uses:

- Circular scrolling logic
- Dynamic theming
- Custom interpolation
- Gradient backgrounds
- Item animations

## Usage

```tsx
// Basic usage with configuration<InfiniteCircularCarousel  ref={carouselRef}  data={ThemeData}  listItemWidth={ListItemSize}  centered  snapEnabled  onActiveIndexChanged={(index) => {    // Handle index change  }}  interpolateConfig={{    inputRange: (index) => [      (index - 2) * ListItemSize,      (index - 1) * ListItemSize,      index * ListItemSize,      (index + 1) * ListItemSize,      (index + 2) * ListItemSize,    ],    outputRange: () => [-1, -1.5, 0, 1.5, 1],    extrapolationType: Extrapolation.CLAMP,  }}  renderItem={({ item, index, progress }) => (    <ListItemCard      item={item}      index={index}      progress={progress}      onPress={() => {        carouselRef.current?.scrollToIndex(index);      }}    />  )}/>
```

GitHubAsk for support

Infinite Carousel - FeedbackShare Your ThoughtsI value a lot your feedback! Help me improve by sharing your thoughts, suggestions, or reporting any issues you encounter. If you need assistance, send me an email at hello@reactiive.ioSend Feedback

---

*Documentation extracted from reactiive.io/demos*
