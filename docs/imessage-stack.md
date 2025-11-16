# iMessageStack

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/imessage-stack)
> **Source Code**: [/src/animations/imessage-stack](/src/animations/imessage-stack)

## Tags
- `reanimated`

## What's This About?

This component creates a horizontally scrollable stack of cards that mimics the behavior of iMessage's media browser. It uses a single ScrollView with paging enabled to handle an infinite number of cards smoothly. The implementation focuses on performance and smooth animations by leveraging native scroll behavior instead of custom gesture handlers. Each card can be customized with different colors and content.

## Technical Implementation

The component uses:

- Reanimated ScrollView
- Paging behavior
- Scroll offset tracking
- Card positioning
- Custom styling

## Usage

```tsx
// Card configurationconst CARD_HEIGHT = 100;const CARD_WIDTH = 100;
// Sample cards dataconst CARDS = [  { color: '#F1EEE0' },  { color: '#F3D9BC' },  { color: '#F4ACB7' },  // ... more cards];
// Basic usage<IMessageStack />
// ScrollView configuration<Animated.ScrollView  horizontal  snapToInterval={CARD_WIDTH}  disableIntervalMomentum  pagingEnabled  showsHorizontalScrollIndicator={false}  decelerationRate="fast"/>
```

GitHubAsk for support

Imessage Stack - FeedbackShare Your ThoughtsI value a lot your feedback! Help me improve by sharing your thoughts, suggestions, or reporting any issues you encounter. If you need assistance, send me an email at hello@reactiive.ioSend Feedback

---

*Documentation extracted from reactiive.io/demos*
