# Stacked Carousel

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/stacked-carousel)
> **Source Code**: [/src/animations/stacked-carousel](/src/animations/stacked-carousel)

## Tags
- `reanimated`

## What it does

Picture a deck of cards spread out in your hand. As you flip through them, each card rotates and scales naturally. That's what this component recreates digitally.

The cards don't just slide left and right - they tilt with perspective rotation, the active card scales up while others shrink down, and there's this nice organic fade where cards move up and down as they transition. The whole thing feels pretty smooth.

There's also a paginator at the bottom that shows which card you're on, with dots that scale and fade based on your position.

## Usage

```tsx
import { StackedCarousel } from './components/stacked-carousel';
const data = [  { id: 1, title: 'Card 1' },  { id: 2, title: 'Card 2' },  { id: 3, title: 'Card 3' },];
const renderCard = (item) => (  <View style={{ flex: 1, backgroundColor: 'white', padding: 20 }}>    <Text>{item.title}</Text>  </View>);
<StackedCarousel  data={data}  renderCard={renderCard}  cardWidth={320}  cardHeight={200}  showPaginator/>;
```

## Technical details

Built with React Native Reanimated for the animations. The tricky part was getting the perspective transforms right - there's a lot of interpolation happening to make the rotation and scaling feel natural.

I used an invisible ScrollView on top to handle the actual scrolling, while the visual cards are positioned absolutely behind it. This way you get native scroll performance but full control over the card animations.

The z-index stacking is calculated so cards layer properly throughout the animation. Each card knows its position in the stack and animates accordingly.

If you're using this in a real app, you'd probably want to add some optimizations for large datasets.

GitHubAsk for support

Stacked Carousel - FeedbackShare Your ThoughtsI value a lot your feedback! Help me improve by sharing your thoughts, suggestions, or reporting any issues you encounter. If you need assistance, send me an email at hello@reactiive.ioSend Feedback

---

*Documentation extracted from reactiive.io/demos*
