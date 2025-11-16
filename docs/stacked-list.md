# Stacked List

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/stacked-list)
> **Source Code**: [/src/animations/stacked-list](/src/animations/stacked-list)

## Tags
- `reanimated`

## What's This About?

This component creates a sophisticated scrollable list where items stack and scale based on their position in the viewport. It features smooth animations for item transitions, with items scaling and transforming as they move through the list. The implementation includes precise interpolation for visibility and transformation calculations, making it perfect for dynamic list interfaces with engaging visual effects.

## Technical Implementation

The component uses:

- Scroll handling
- Position interpolation
- Scale animations
- Visibility calculations
- Transform effects

## Usage

```tsx
// Basic usage<StackedList />;
// List item configurationconst ListConfig = {  itemHeight: 100,  margin: 10,  marginTop: 70,  offset: 80,};
// List item componentconst ListItem = ({  index,  scrollOffset,}: {  index: number;  scrollOffset: SharedValue<number>;}) => {  const baseTranslateY = index * (ListConfig.itemHeight + ListConfig.margin);
  // Visibility calculation  const visibleAmount = useDerivedValue(() => {    const distanceFromTop =      scrollOffset.value +      (ScreenHeight - ListConfig.marginTop - ListConfig.offset) -      baseTranslateY;
    return interpolate(      distanceFromTop,      [0, ListConfig.itemHeight + ListConfig.margin],      [0, ListConfig.itemHeight + ListConfig.margin],      Extrapolation.EXTEND    );  }, []);
  // Scale animation  const scale = useDerivedValue(() => {    return interpolate(      visibleAmount.value,      [0, ListConfig.itemHeight + ListConfig.margin],      [0.6, 1],      Extrapolation.CLAMP    );  }, []);};
```

GitHubAsk for support

Stacked List - FeedbackShare Your ThoughtsI value a lot your feedback! Help me improve by sharing your thoughts, suggestions, or reporting any issues you encounter. If you need assistance, send me an email at hello@reactiive.ioSend Feedback

---

*Documentation extracted from reactiive.io/demos*
