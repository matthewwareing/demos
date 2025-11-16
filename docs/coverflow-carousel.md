# Coverflow Carousel

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/coverflow-carousel)
> **Source Code**: [/src/animations/coverflow-carousel](/src/animations/coverflow-carousel)

## Tags
- `reanimated`

## What's This About?

This component creates an advanced carousel where images smoothly transform as they move through different positions. Each image dynamically adjusts its scale, position, opacity, and border radius based on its position in the carousel, creating a fluid and engaging visual experience.

## Technical Implementation

The component implements sophisticated animations using Reanimated:

- Complex interpolations for multiple properties:Scale transformations in both X and Y axesDynamic position adjustmentsSmooth opacity transitionsAdaptive border radius changes
- Scale transformations in both X and Y axes
- Dynamic position adjustments
- Smooth opacity transitions
- Adaptive border radius changes
- Optimized FlatList with custom scroll behavior
- Precise item measurements and positioning
- Expo Image component for efficient image loading

## Usage

```tsx
type CoverFlowCarouselProps = {  images: string[];  // Array of image URLs};
// Basic usage<CoverFlowCarousel  images={[    'https://example.com/image1.jpg',    'https://example.com/image2.jpg',    // ...more images  ]}/>
// The component handles:// - Automatic item sizing (160px width)// - Center alignment// - Smooth scrolling with snap points// - Fast deceleration for crisp stops

<GitHubRepoButtons />
<SendFeedback />
```

---

*Documentation extracted from reactiive.io/demos*
