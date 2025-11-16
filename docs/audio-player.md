# AudioPlayer

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/audio-player)
> **Source Code**: [/src/animations/audio-player](/src/animations/audio-player)

## Tags
- `reanimated`

## What's This About?

This component creates an interactive audio waveform display where users can scrub through the audio content. The waveform responds to touch gestures, providing visual feedback as users navigate through the track, while a time display updates in real-time.

## Technical Implementation

The component uses gesture handling for smooth scrubbing interactions and derived values for time calculations. It features a dynamic waveform visualization that responds to the current playback position and user interaction state.

## Usage

```tsx
type WaveformScrubberProps = {  waveformSamples: number[];  // Array of amplitude values};
// Example usage<WaveformScrubber  waveformSamples={[0.5, 0.8, 0.3, ...]} // Amplitude values between 0 and 1/>
```

GitHubAsk for support

Audio Player - FeedbackShare Your ThoughtsI value a lot your feedback! Help me improve by sharing your thoughts, suggestions, or reporting any issues you encounter. If you need assistance, send me an email at hello@reactiive.ioSend Feedback

---

*Documentation extracted from reactiive.io/demos*
