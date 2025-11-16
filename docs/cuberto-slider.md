# Cuberto Slider

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/cuberto-slider)
> **Source Code**: [/src/animations/cuberto-slider](/src/animations/cuberto-slider)

## Tags
- `reanimated`
- `gesture-handler`

## What's This About?

This component creates an interactive slider with a unique visual style and smooth animations. The slider responds to user gestures with fluid transitions and provides visual feedback through elegant animations, making it perfect for settings, preferences, or any numerical input.

## Technical Implementation

The component leverages gesture handling and animations to create a polished experience:

- Gesture-based interactions
- Smooth value transitions
- Custom styling and theming
- Performance optimizations with React.memo
- Responsive layout adaptations

## Usage

```tsx
// Basic usage with default settings<CubertoSlider />
// Custom implementation<Slider  min={0}  max={100}  step={1}  onValueChange={(value) => {    console.log('Current value:', value);  }}/>
// With gesture handler root<GestureHandlerRootView>  <CubertoSlider /></GestureHandlerRootView>
```

GitHubAsk for support

Cuberto Slider - FeedbackShare Your ThoughtsI value a lot your feedback! Help me improve by sharing your thoughts, suggestions, or reporting any issues you encounter. If you need assistance, send me an email at hello@reactiive.ioSend Feedback

---

*Documentation extracted from reactiive.io/demos*
