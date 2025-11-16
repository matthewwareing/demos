# Verification Code Face

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/verification-code-face)
> **Source Code**: [/src/animations/verification-code-face](/src/animations/verification-code-face)

## Tags
- `reanimated`
- `skia`

### The Face

The Face is a Square with:

- 2 Eyebrows: I used a Skia Path to draw the eyebrows
- 2 Eyes: I used multiple Animated.Views to draw and animate the eyes
- 1 Mouth: I used a Skia Path to draw the mouth

To animate the Path I built manually the expected paths as SVGs.

```tsx
const createPath = (  type: 'Happy' | 'Sad' | 'Normal',  { height, width }: PathParams) => {  switch (type) {    case 'Happy':      return `M0 ${height / 2} Q${width / 2} ${height} ${width} ${height / 2}`;    case 'Sad':      return `M0 ${height / 2} Q${width / 2} 0 ${width} ${height / 2}`;    case 'Normal':      return `M0 ${height / 2} Q${width / 2} ${height / 2} ${width} ${        height / 2      }`;  }};
export const DefaultMouthPaths = {  Happy: createPath('Happy', { height: MOUTH_HEIGHT, width: MOUTH_WIDTH }),  Sad: createPath('Sad', { height: MOUTH_HEIGHT, width: MOUTH_WIDTH }),  Normal: createPath('Normal', { height: MOUTH_HEIGHT, width: MOUTH_WIDTH }),};
export const DefaultEyebrowPaths = {  // Note how the Happy Eyebrow is just the Sad Mouth flipped 😅  Happy: createPath('Sad', { height: EYEBROW_HEIGHT, width: EYEBROW_WIDTH }),  Sad: createPath('Happy', { height: EYEBROW_HEIGHT, width: EYEBROW_WIDTH }),  Normal: createPath('Normal', {    height: EYEBROW_HEIGHT,    width: EYEBROW_WIDTH,  }),};
```

Then it was just a matter of animating the paths using the usePathInterpolation hook from Skia.

```typescript
const activeMouthPath = usePathInterpolation(  animatedProgress,  [AnimationType.Happy, AnimationType.Normal, AnimationType.Sad],  outputRange);
```

Again, there are simpler ways to handle this animation, but I think it is cool to see how to use Skia since in the very end it gives you a tremendous amount of control.

It's crazy how shifting a bit the eyes/mouth/eyebrows can create different faces.

GitHubAsk for support

Verification Code Face - FeedbackShare Your ThoughtsI value a lot your feedback! Help me improve by sharing your thoughts, suggestions, or reporting any issues you encounter. If you need assistance, send me an email at hello@reactiive.ioSend Feedback

---

*Documentation extracted from reactiive.io/demos*
