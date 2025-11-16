# iMessageStack

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/imessage-stack)
> **Source Code**: [/src/animations/imessage-stack](/src/animations/imessage-stack)

## Tags
- `reanimated`

## Description

Scan to try on your device

## Technical Implementation

- Reanimated ScrollView
- Paging behavior
- Scroll offset tracking
- Card positioning
- Custom styling

## Usage

```typescript
// Card configurationconst CARD_HEIGHT = 100;const CARD_WIDTH = 100;
// Sample cards dataconst CARDS = [  { color: '#F1EEE0' },  { color: '#F3D9BC' },  { color: '#F4ACB7' },  // ... more cards];
// Basic usage<IMessageStack />
// ScrollView configuration<Animated.ScrollView  horizontal  snapToInterval={CARD_WIDTH}  disableIntervalMomentum  pagingEnabled  showsHorizontalScrollIndicator={false}  decelerationRate="fast"/>
```

---

*Documentation extracted from reactiive.io/demos*
