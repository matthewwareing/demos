# Circular Carousel

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/circular-carousel)
> **Source Code**: [/src/animations/circular-carousel](/src/animations/circular-carousel)

## Tags
- `reanimated`

## What's This About?

This component creates an interactive circular carousel where images are arranged in a circle. Users can rotate through the images with smooth animations, and an optional scaling effect can be toggled to enhance the visual experience.

## Technical Implementation

The component implements:

- Circular layout arrangement
- Smooth rotation animations
- Optional scale effects
- Image preloading and optimization
- Touch gesture handling
- Configurable visual options

## Usage

```tsx
type CircularListProps = {  data: string[];  // Array of image URLs  scaleEnabled: boolean;};
// Basic usage<CircularCarousel />
// Custom implementation<CircularList  data={[    'https://example.com/image1.jpg',    'https://example.com/image2.jpg',    // ...more images  ]}  scaleEnabled={true}/>
```

GitHubAsk for support

Circular Carousel - FeedbackShare Your ThoughtsI value a lot your feedback! Help me improve by sharing your thoughts, suggestions, or reporting any issues you encounter. If you need assistance, send me an email at hello@reactiive.ioSend Feedback

---

*Documentation extracted from reactiive.io/demos*
