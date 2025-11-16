# Verification Code Face

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/verification-code-face)
> **Source Code**: [/src/animations/verification-code-face](/src/animations/verification-code-face)

## Tags
- `reanimated`
- `skia`

## Description

Scan to try on your device

### The Face

- 2 Eyebrows: I used a Skia Path to draw the eyebrows
- 2 Eyes: I used multiple Animated.Views to draw and animate the eyes
- 1 Mouth: I used a Skia Path to draw the mouth

```tsx
const createPath = (  type: 'Happy' | 'Sad' | 'Normal',  { height, width }: PathParams) => {  switch (type) {    case 'Happy':      return `M0 ${height / 2} Q${width / 2} ${height} ${width} ${height / 2}`;    case 'Sad':      return `M0 ${height / 2} Q${width / 2} 0 ${width} ${height / 2}`;    case 'Normal':      return `M0 ${height / 2} Q${width / 2} ${height / 2} ${width} ${        height / 2      }`;  }};
export const DefaultMouthPaths = {  Happy: createPath('Happy', { height: MOUTH_HEIGHT, width: MOUTH_WIDTH }),  Sad: createPath('Sad', { height: MOUTH_HEIGHT, width: MOUTH_WIDTH }),  Normal: createPath('Normal', { height: MOUTH_HEIGHT, width: MOUTH_WIDTH }),};
export const DefaultEyebrowPaths = {  // Note how the Happy Eyebrow is just the Sad Mouth flipped 😅  Happy: createPath('Sad', { height: EYEBROW_HEIGHT, width: EYEBROW_WIDTH }),  Sad: createPath('Happy', { height: EYEBROW_HEIGHT, width: EYEBROW_WIDTH }),  Normal: createPath('Normal', {    height: EYEBROW_HEIGHT,    width: EYEBROW_WIDTH,  }),};
```

```typescript
const activeMouthPath = usePathInterpolation(  animatedProgress,  [AnimationType.Happy, AnimationType.Normal, AnimationType.Sad],  outputRange);
```

---

*Documentation extracted from reactiive.io/demos*
