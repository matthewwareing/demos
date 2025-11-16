# Airbnb Flip Interaction

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/airbnb-flip-interaction)
> **Source Code**: [/src/animations/airbnb-flip-interaction](/src/animations/airbnb-flip-interaction)

## Tags
- `reanimated`
- `expo-blur`

## Description

An interactive profile card that flips like a real credit card. Tap it to see smooth 3D animations as it rotates to show more details on the back.

## What it does

Picture flipping over a credit card to read the details on the back. That's exactly what this component does, but digitally.

The front shows a colorful card with the person's name and photo. Tap it, and watch it smoothly flip over to reveal stats like how many trips they've taken and places they've visited. Everything feels smooth and natural.

Below the card, there's text that changes depending on which side you're looking at. During the flip, the background gets a nice blur effect to keep your focus on the card animation.

## Usage

```tsx
import { FlipCard } from './flip-interaction';
import type { ProfileType } from './flip-interaction/components/card/types';

const profile: ProfileType = {
  name: 'John Doe',
  location: 'San Francisco',
  trips: 12,
  reviews: 8,
  yearsOnAirbnb: 3,
  birthDecade: 'Born in the 90s',
  languages: ['Speaks English', 'Speaks Spanish'],
  isIdentityVerified: true,
  visitedPlaces: [
    {
      name: 'Paris',
      country: 'Paris, France',
      code: 'FR',
    },
    {
      name: 'Tokyo',
      country: 'Tokyo, Japan',
      code: 'JP',
    },
    // ... more places
  ],
};

export default function App() {
  return <FlipCard profile={profile} />;
}
```

## Key Features

- **3D Flip Animation**: Smooth card flip using Reanimated transforms
- **Blur Effect**: Background blur during flip animation using expo-blur
- **Interactive**: Tap to flip between front and back
- **Responsive**: Adapts to different screen sizes
- **Type-Safe**: Full TypeScript support

## Technical Implementation

The flip animation uses:
- `useSharedValue` and `useAnimatedStyle` from Reanimated
- `rotateY` transform for the 3D flip effect
- Interpolation to sync multiple animations
- Blur intensity tied to flip progress

---

*Documentation extracted from reactiive.io/demos*
