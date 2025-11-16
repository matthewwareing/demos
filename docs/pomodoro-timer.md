# Pomodoro Timer

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/pomodoro-timer)
> **Source Code**: [/src/animations/pomodoro-timer](/src/animations/pomodoro-timer)

## Tags
- `reanimated`

## What's This About?

This component creates an interactive Pomodoro timer with a circular draggable interface. Users can set the timer duration by dragging along a circular slider, with haptic feedback for precise control. The component features an animated count display, customizable visual elements, and completion alerts. The timer can be started, stopped, and reset, making it perfect for time management applications.

## Technical Implementation

The component uses:

- Circular slider
- Haptic feedback
- Animated counting
- Timer controls
- Completion alerts

## Usage

```tsx
// Basic usage<PomodoroTimer />
// Animated count display<AnimatedCount  count={animatedNumber}  maxDigits={5}  textDigitWidth={68}  textDigitHeight={120}  fontSize={100}  color="#fff"  gradientAccentColor="#000"/>
// Circular slider<CircularDraggableSlider  linesAmount={200}  indicatorColor="orange"  maxLineHeight={40}  lineColor="rgba(255,255,255,0.5)"  bigLineColor="white"  minLineHeight={30}  onCompletion={() => {    // Handle timer completion  }}  onProgressChange={(progress) => {    // Handle progress updates  }}/>
```

GitHubAsk for support

Pomodoro Timer - FeedbackShare Your ThoughtsI value a lot your feedback! Help me improve by sharing your thoughts, suggestions, or reporting any issues you encounter. If you need assistance, send me an email at hello@reactiive.ioSend Feedback

---

*Documentation extracted from reactiive.io/demos*
