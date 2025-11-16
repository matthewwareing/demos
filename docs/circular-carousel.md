# Circular Carousel

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/circular-carousel)
> **Source Code**: [/src/animations/circular-carousel](/src/animations/circular-carousel)

## Tags
- `reanimated`

## Description

Scan to try on your device

## Technical Implementation

- Circular layout arrangement
- Smooth rotation animations
- Optional scale effects
- Image preloading and optimization
- Touch gesture handling
- Configurable visual options

## Usage

```typescript
type CircularListProps = {  data: string[];  // Array of image URLs  scaleEnabled: boolean;};
// Basic usage<CircularCarousel />
// Custom implementation<CircularList  data={[    'https://example.com/image1.jpg',    'https://example.com/image2.jpg',    // ...more images  ]}  scaleEnabled={true}/>
```

---

*Documentation extracted from reactiive.io/demos*
