# Dot Sheet

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/dot-sheet)
> **Source Code**: [/src/animations/dot-sheet](/src/animations/dot-sheet)

## Tags
- `reanimated`
- `skia`

## Description

Scan to try on your device

## What's This About?

- Bottom sheet for card details
- Gradient background
- Call-to-action button
- Safe area handling

## Technical Implementation

- Reanimated for animations
- Gradient background with Skia
- Custom font integration
- Bottom sheet gestures
- Ref-based focus management

## Usage

```typescript
// Basic usage<DotSheet />;
// Card input referenceconst cardInputRef = useRef<CardInputRefType>(null);
// Component structure<>  <BackgroundGradient />  <CardInput ref={cardInputRef} />  <PressableScale    onPress={() => {      cardInputRef.current?.focus();    }}  >    <Text>Start your Journey</Text>  </PressableScale></>;
```

---

*Documentation extracted from reactiive.io/demos*
