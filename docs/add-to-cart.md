# Add to Cart

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/add-to-cart)
> **Source Code**: [/src/animations/add-to-cart](/src/animations/add-to-cart)

## Tags
- `reanimated`
- `gesture-handler`

## What's This About?

The animation creates an engaging shopping experience by combining a product grid with smooth transitions and a detailed view when selecting items. Each interaction is accompanied by fluid animations that provide visual feedback for the user's actions.

## Core Components

The animation consists of a main list view that displays products, an animated bottom sheet for item details, and a dynamic confirmation button. When an item is selected, the bottom sheet slides up smoothly while the background dims to focus attention on the active content.

## Technical Implementation

The component uses shared values and interpolated animations for state management. It handles layout measurements to ensure precise positioning and implements cancellable animations for a better user experience.

## Usage

```typescript
type Item = {  id: number;  title: string;  imageUri: string;  description: string;  count: number;};
// The component automatically manages item selection and cart quantities
```

GitHubAsk for support

Add To Cart - FeedbackShare Your ThoughtsI value a lot your feedback! Help me improve by sharing your thoughts, suggestions, or reporting any issues you encounter. If you need assistance, send me an email at hello@reactiive.ioSend Feedback

---

*Documentation extracted from reactiive.io/demos*
