# AirBnb Slider

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/airbnb-slider)
> **Source Code**: [/src/animations/airbnb-slider](/src/animations/airbnb-slider)

## Tags
- `reanimated`
- `gesture-handler`

## What's This About?

This component recreates Airbnb's price selector with animated transitions for both the slider and price display. As users adjust the slider, the price updates with a rolling number animation while the currency symbol smoothly repositions itself.

## Technical Implementation

The component uses spring animations for natural movement and shared values for state management. The price display intelligently handles digit spacing and currency positioning, while the slider provides smooth, responsive feedback.

## Usage

```tsx
// The component accepts these main propstype Props = {  initialProgress?: number;  minValue?: number;  maxValue: number;  onUpdate: (value: number) => void;};
// Example usage<AirbnbSlider maxValue={4500} onUpdate={(price) => console.log(price)} />;
```

GitHubAsk for support

Airbnb Slider - FeedbackShare Your ThoughtsI value a lot your feedback! Help me improve by sharing your thoughts, suggestions, or reporting any issues you encounter. If you need assistance, send me an email at hello@reactiive.ioSend Feedback

---

*Documentation extracted from reactiive.io/demos*
