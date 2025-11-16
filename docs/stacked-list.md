# Stacked List

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/stacked-list)
> **Source Code**: [/src/animations/stacked-list](/src/animations/stacked-list)

## Tags
- `reanimated`

## Description

Scan to try on your device

## Technical Implementation

- Scroll handling
- Position interpolation
- Scale animations
- Visibility calculations
- Transform effects

## Usage

```typescript
// Basic usage<StackedList />;
// List item configurationconst ListConfig = {  itemHeight: 100,  margin: 10,  marginTop: 70,  offset: 80,};
// List item componentconst ListItem = ({  index,  scrollOffset,}: {  index: number;  scrollOffset: SharedValue<number>;}) => {  const baseTranslateY = index * (ListConfig.itemHeight + ListConfig.margin);
  // Visibility calculation  const visibleAmount = useDerivedValue(() => {    const distanceFromTop =      scrollOffset.value +      (ScreenHeight - ListConfig.marginTop - ListConfig.offset) -      baseTranslateY;
    return interpolate(      distanceFromTop,      [0, ListConfig.itemHeight + ListConfig.margin],      [0, ListConfig.itemHeight + ListConfig.margin],      Extrapolation.EXTEND    );  }, []);
  // Scale animation  const scale = useDerivedValue(() => {    return interpolate(      visibleAmount.value,      [0, ListConfig.itemHeight + ListConfig.margin],      [0.6, 1],      Extrapolation.CLAMP    );  }, []);};
```

---

*Documentation extracted from reactiive.io/demos*
