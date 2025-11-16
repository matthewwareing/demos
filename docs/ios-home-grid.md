# iOS Home Grid

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/ios-home-grid)
> **Source Code**: [/src/animations/ios-home-grid](/src/animations/ios-home-grid)

## Tags
- `reanimated`
- `gesture-handler`
- `expo-blur`

## Description

Scan to try on your device

## How It Works

- Touch Detection - Captures tap location using React Native Gesture Handler
- Position Measurement - Gets icon dimensions and position using layout measurements
- Expansion Animation - Scales up the icon using spring physics with Reanimated
- Border Radius - Animates border radius from icon corners to full screen
- Navigation - Handles screen transitions and back gesture interactions

### How the Code is Organized

```typescript
src/├── apps-list/│   ├── index.tsx           → The main grid that shows all the app icons│   ├── app-item.tsx        → Each individual app icon component│   └── constants.ts        → All the beautiful gradient color combinations├── navigation/│   ├── expansion-provider.tsx    → The brain that orchestrates all animations│   ├── navigation-item.tsx       → Handles taps and triggers transitions│   ├── MainScreenWrapper.tsx     → Wraps the home screen with special powers│   └── DetailScreenWrapper.tsx   → Wraps the detail screen for smooth exits├── app-detail-screen.tsx   → The full-screen view you see after tapping└── index.tsx              → Brings everything together with navigation
```

---

*Documentation extracted from reactiive.io/demos*
