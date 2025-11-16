# Animated 3D Parallax

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/animated-3d-parallax)
> **Source Code**: [/src/animations/animated-3d-parallax](/src/animations/animated-3d-parallax)

## Tags
- `reanimated`
- `gesture-handler`

## What's This About?

This component creates an immersive 3D effect where touch input controls the card's rotation. The content follows with a slight delay, creating a parallax effect that adds depth to the interaction. The result is a polished, iOS-like 3D card that responds naturally to user input.

## Technical Implementation

The component uses spring animations and gesture handling for smooth interactions. It implements custom 3D rotation calculations with perspective transforms and interpolated values to achieve realistic motion.

## Usage

```tsx
type Use3DRotationStyleParams = {  x: Animated.SharedValue<number>;  y: Animated.SharedValue<number>;  maxSize: number;  maxRotation: number;};
// Example usage<Animated3DParallax />;
```

GitHubAsk for support

Animated 3d Parallax - FeedbackShare Your ThoughtsI value a lot your feedback! Help me improve by sharing your thoughts, suggestions, or reporting any issues you encounter. If you need assistance, send me an email at hello@reactiive.ioSend Feedback

---

*Documentation extracted from reactiive.io/demos*
