# Coverflow Carousel

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/coverflow-carousel)
> **Source Code**: [/src/animations/coverflow-carousel](/src/animations/coverflow-carousel)

## Tags
- `reanimated`

## Description

Scan to try on your device

## Technical Implementation

- Complex interpolations for multiple properties:Scale transformations in both X and Y axesDynamic position adjustmentsSmooth opacity transitionsAdaptive border radius changes
- Scale transformations in both X and Y axes
- Dynamic position adjustments
- Smooth opacity transitions
- Adaptive border radius changes
- Optimized FlatList with custom scroll behavior
- Precise item measurements and positioning
- Expo Image component for efficient image loading

## Usage

```typescript
type CoverFlowCarouselProps = {  images: string[];  // Array of image URLs};
// Basic usage<CoverFlowCarousel  images={[    'https://example.com/image1.jpg',    'https://example.com/image2.jpg',    // ...more images  ]}/>
// The component handles:// - Automatic item sizing (160px width)// - Center alignment// - Smooth scrolling with snap points// - Fast deceleration for crisp stops

<GitHubRepoButtons />
<SendFeedback />
```

---

*Documentation extracted from reactiive.io/demos*
