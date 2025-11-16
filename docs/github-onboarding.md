# GitHub Onboarding

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/github-onboarding)
> **Source Code**: [/src/animations/github-onboarding](/src/animations/github-onboarding)

## Tags
- `reanimated`

## Description

Scan to try on your device

## Technical Implementation

- Gesture handling
- Image transitions
- Color interpolation
- Dynamic data rendering
- Screen navigation

## Usage

```typescript
// Data structuretype OnboardingItem = {  title: string;  color: string;  image: ImageSourcePropType;};
// Sample dataconst data = [  {    title: 'Lazy Day Lounger',    color: '#265D9E',    image: require('./assets/02.jpg'),  },  {    title: 'Whiskered Explorer',    color: '#4E8DC5',    image: require('./assets/01.jpg'),  },];
// Basic usage<ColorfulOnboarding data={data} />;
```

---

*Documentation extracted from reactiive.io/demos*
