# Wheel Picker

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/wheel-picker)
> **Source Code**: [/src/animations/wheel-picker](/src/animations/wheel-picker)

## Tags
- `reanimated`
- `gesture-handler`

## What's This About?

This component creates an interactive wheel picker with an animated number display and a draggable slider. It features expandable line spacing, smooth animations, and precise value selection. The implementation includes a customizable slider with gradient boundaries, animated count display, and responsive layout, making it perfect for numeric value selection or any interface requiring precise control over numerical values.

## Technical Implementation

The component uses:

- Animated counting
- Draggable slider
- Space animation
- Progress tracking
- Gradient boundaries

## Usage

```tsx
// Basic usage<WheelPicker />
// Animated count display<AnimatedCount  count={animatedNumber}  maxDigits={10}  textDigitWidth={44}  textDigitHeight={80}  fontSize={65}/>
// Draggable slider<DraggableSlider  scrollableAreaHeight={150}  spacePerLine={animatedSpacePerLine}  showBoundaryGradient  bigLineIndexOffset={20}  snapEach={1}  linesAmount={50}  maxLineHeight={20}  minLineHeight={10}  onProgressChange={(progress) => {    'worklet';    if (progress < 0) return;    animatedValue.value = progress;  }}/>
// Space animationconst animatedSpacePerLine = useDerivedValue(() => {  return withTiming(isExpanded ? 50 : 20);}, [isExpanded]);
// Progress trackingconst progress = useSharedValue(0);const animatedNumber = useDerivedValue(() => {  const multiplier = 1;  return Math.ceil(    progress.value * LinesAmount * multiplier  );}, [progress]);
```

GitHubAsk for support

Wheel Picker - FeedbackShare Your ThoughtsI value a lot your feedback! Help me improve by sharing your thoughts, suggestions, or reporting any issues you encounter. If you need assistance, send me an email at hello@reactiive.ioSend Feedback

---

*Documentation extracted from reactiive.io/demos*
