# GitHub Onboarding

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/github-onboarding)
> **Source Code**: [/src/animations/github-onboarding](/src/animations/github-onboarding)

## Tags
- `reanimated`

## What's This About?

This component creates an engaging onboarding experience inspired by GitHub's design patterns. It features a series of screens with smooth transitions between images, each accompanied by a title and a dynamic color scheme. The component automatically handles gesture-based navigation and provides visual feedback through color transitions that complement each screen's content.

## Technical Implementation

The component uses:

- Gesture handling
- Image transitions
- Color interpolation
- Dynamic data rendering
- Screen navigation

## Usage

```tsx
// Data structuretype OnboardingItem = {  title: string;  color: string;  image: ImageSourcePropType;};
// Sample dataconst data = [  {    title: 'Lazy Day Lounger',    color: '#265D9E',    image: require('./assets/02.jpg'),  },  {    title: 'Whiskered Explorer',    color: '#4E8DC5',    image: require('./assets/01.jpg'),  },];
// Basic usage<ColorfulOnboarding data={data} />;
```

GitHubAsk for support

Github Onboarding - FeedbackShare Your ThoughtsI value a lot your feedback! Help me improve by sharing your thoughts, suggestions, or reporting any issues you encounter. If you need assistance, send me an email at hello@reactiive.ioSend Feedback

---

*Documentation extracted from reactiive.io/demos*
