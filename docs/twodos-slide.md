# Twodos Slide

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/twodos-slide)
> **Source Code**: [/src/animations/twodos-slide](/src/animations/twodos-slide)

## Tags
- `reanimated`
- `gesture-handler`
- `skia`

## What's This About?

This component creates an interactive slide-to-unlock interface with animated squares that respond to the sliding gesture. It features a friction slider with haptic feedback, debounced interactions, and smooth animations. The implementation includes gesture handling, progress tracking, and visual feedback through animated squares, making it perfect for unlock screens or interactive sliders requiring visual feedback.

## Technical Implementation

The component uses:

- Gesture handling
- Haptic feedback
- Progress tracking
- Animated squares
- Debounced interactions

## Usage

```tsx
// Basic usage<TwodosSlide />
// Friction slider with progress tracking<FrictionSlider  containerStyle={styles.container}  onProgressChange={({    clampedProgress,    realProgress  }) => {    'worklet';    if (progress.value >= 1) {      runOnJS(debouncedHapticFeedback)();    }    progress.value = realProgress;    clampedProgress.value = clampedProgress;  }}>  <Text>Slide to Unlock</Text>  <AntDesign name="arrowright" size={20} color="gray" /></FrictionSlider>
// Animated squares<AnimatedSquares  clampedProgress={clampedProgress}  progress={progress}  size={120}/>
// Debounced haptic feedbackconst debouncedHapticFeedback = useMemo(  () => debounce(hapticFeedback, 1000, {    leading: true,    trailing: false  }),  []);
// Progress trackingconst progress = useSharedValue(0);const clampedProgress = useSharedValue(0);
```

GitHubAsk for support

Twodos Slide - FeedbackShare Your ThoughtsI value a lot your feedback! Help me improve by sharing your thoughts, suggestions, or reporting any issues you encounter. If you need assistance, send me an email at hello@reactiive.ioSend Feedback

---

*Documentation extracted from reactiive.io/demos*
