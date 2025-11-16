# Twodos Slide

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/twodos-slide)
> **Source Code**: [/src/animations/twodos-slide](/src/animations/twodos-slide)

## Tags
- `reanimated`
- `gesture-handler`
- `skia`

## Description

Scan to try on your device

## Technical Implementation

- Gesture handling
- Haptic feedback
- Progress tracking
- Animated squares
- Debounced interactions

## Usage

```typescript
// Basic usage<TwodosSlide />
// Friction slider with progress tracking<FrictionSlider  containerStyle={styles.container}  onProgressChange={({    clampedProgress,    realProgress  }) => {    'worklet';    if (progress.value >= 1) {      runOnJS(debouncedHapticFeedback)();    }    progress.value = realProgress;    clampedProgress.value = clampedProgress;  }}>  <Text>Slide to Unlock</Text>  <AntDesign name="arrowright" size={20} color="gray" /></FrictionSlider>
// Animated squares<AnimatedSquares  clampedProgress={clampedProgress}  progress={progress}  size={120}/>
// Debounced haptic feedbackconst debouncedHapticFeedback = useMemo(  () => debounce(hapticFeedback, 1000, {    leading: true,    trailing: false  }),  []);
// Progress trackingconst progress = useSharedValue(0);const clampedProgress = useSharedValue(0);
```

---

*Documentation extracted from reactiive.io/demos*
