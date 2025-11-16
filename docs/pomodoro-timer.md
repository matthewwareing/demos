# Pomodoro Timer

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/pomodoro-timer)
> **Source Code**: [/src/animations/pomodoro-timer](/src/animations/pomodoro-timer)

## Tags
- `reanimated`

## Description

Scan to try on your device

## Technical Implementation

- Circular slider
- Haptic feedback
- Animated counting
- Timer controls
- Completion alerts

## Usage

```typescript
// Basic usage<PomodoroTimer />
// Animated count display<AnimatedCount  count={animatedNumber}  maxDigits={5}  textDigitWidth={68}  textDigitHeight={120}  fontSize={100}  color="#fff"  gradientAccentColor="#000"/>
// Circular slider<CircularDraggableSlider  linesAmount={200}  indicatorColor="orange"  maxLineHeight={40}  lineColor="rgba(255,255,255,0.5)"  bigLineColor="white"  minLineHeight={30}  onCompletion={() => {    // Handle timer completion  }}  onProgressChange={(progress) => {    // Handle progress updates  }}/>
```

---

*Documentation extracted from reactiive.io/demos*
