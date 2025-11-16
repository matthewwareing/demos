# Paper Folding

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/paper-folding)
> **Source Code**: [/src/animations/paper-folding](/src/animations/paper-folding)

## Tags
- `skia`

## Description

Scan to try on your device

## Technical Implementation

- Touch handling
- Timing animations
- Gradient backgrounds
- Paper folding effects
- Dimension control

## Usage

```typescript
// Basic usage<PaperFolding />;
// Component configurationconst PaperWidth = 250;const PaperHeight = 330;
// Animation controlconst progress = useSharedValue(0);
// Paper component with props<Paper width={PaperWidth} height={PaperHeight} progress={progress} />;
// Animation triggerprogress.value = withTiming(progress.value > 0 ? 0 : 1, {  duration: 800,});
```

---

*Documentation extracted from reactiive.io/demos*
