# Wheel Picker

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/wheel-picker)
> **Source Code**: [/src/animations/wheel-picker](/src/animations/wheel-picker)

## Tags
- `reanimated`
- `gesture-handler`

## Description

Scan to try on your device

## Technical Implementation

- Animated counting
- Draggable slider
- Space animation
- Progress tracking
- Gradient boundaries

## Usage

```typescript
// Basic usage<WheelPicker />
// Animated count display<AnimatedCount  count={animatedNumber}  maxDigits={10}  textDigitWidth={44}  textDigitHeight={80}  fontSize={65}/>
// Draggable slider<DraggableSlider  scrollableAreaHeight={150}  spacePerLine={animatedSpacePerLine}  showBoundaryGradient  bigLineIndexOffset={20}  snapEach={1}  linesAmount={50}  maxLineHeight={20}  minLineHeight={10}  onProgressChange={(progress) => {    'worklet';    if (progress < 0) return;    animatedValue.value = progress;  }}/>
// Space animationconst animatedSpacePerLine = useDerivedValue(() => {  return withTiming(isExpanded ? 50 : 20);}, [isExpanded]);
// Progress trackingconst progress = useSharedValue(0);const animatedNumber = useDerivedValue(() => {  const multiplier = 1;  return Math.ceil(    progress.value * LinesAmount * multiplier  );}, [progress]);
```

---

*Documentation extracted from reactiive.io/demos*
