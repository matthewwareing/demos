# Blurred Scroll

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/blurred-scroll)
> **Source Code**: [/src/animations/blurred-scroll](/src/animations/blurred-scroll)

## Tags
- `reanimated`
- `skia`

## What's This About?

This component creates a scrollable list where items dynamically blur and transform based on their position relative to the scroll offset. As users scroll through the list, items smoothly transition between focused and blurred states, creating a depth effect.

## Technical Implementation

The component leverages Reanimated for smooth scroll handling and implements:

- Dynamic blur effects based on scroll position
- Optimized scroll performance with event throttling
- Pre-calculated item layouts for smooth scrolling
- Responsive sizing based on window dimensions
- Fade-in animations for items

## Usage

```tsx
// Core animation setupconst contentOffsetY = useSharedValue(0);const scrollHandler = useAnimatedScrollHandler({  onScroll: (event) => {    contentOffsetY.value = event.contentOffset.y;  },});
// Item configuration<BlurredItem  width={windowWidth}  height={blurredItemContainerHeight}  index={index}  contentOffsetY={contentOffsetY}/>;
```

GitHubAsk for support

Blurred Scroll - FeedbackShare Your ThoughtsI value a lot your feedback! Help me improve by sharing your thoughts, suggestions, or reporting any issues you encounter. If you need assistance, send me an email at hello@reactiive.ioSend Feedback

---

*Documentation extracted from reactiive.io/demos*
