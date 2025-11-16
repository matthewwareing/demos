# Stacked Carousel

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/stacked-carousel)
> **Source Code**: [/src/animations/stacked-carousel](/src/animations/stacked-carousel)

## Tags
- `reanimated`

## Description

Scan to try on your device

## Usage

```tsx
import { StackedCarousel } from './components/stacked-carousel';
const data = [  { id: 1, title: 'Card 1' },  { id: 2, title: 'Card 2' },  { id: 3, title: 'Card 3' },];
const renderCard = (item) => (  <View style={{ flex: 1, backgroundColor: 'white', padding: 20 }}>    <Text>{item.title}</Text>  </View>);
<StackedCarousel  data={data}  renderCard={renderCard}  cardWidth={320}  cardHeight={200}  showPaginator/>;
```

---

*Documentation extracted from reactiive.io/demos*
