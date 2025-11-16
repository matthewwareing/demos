# Shared Transitions

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/shared-transitions)
> **Source Code**: [/src/animations/shared-transitions](/src/animations/shared-transitions)

## Tags
- `reanimated`

## What's This About?

This component implements a navigation stack with smooth shared element transitions between screens. When navigating between the home screen and details screen, elements that appear in both screens can animate smoothly from their position in one screen to their position in the other. The implementation uses React Navigation with custom animation configurations for seamless transitions.

## Technical Implementation

The component uses:

- React Navigation
- Stack navigation
- Shared elements
- Custom animations
- Screen transitions

## Usage

```tsx
// Navigation setupconst Stack = createNativeStackNavigator<RootStackParamsList>();
// Basic usage<Stack.Navigator  initialRouteName="Home"  screenOptions={{    animation: 'fade',    animationDuration: 300,  }}>  <Stack.Screen name="Home" component={HomeScreen} />  <Stack.Screen name="Details" component={DetailsScreen} /></Stack.Navigator>;
// Screen typestype RootStackParamsList = {  Home: undefined;  Details: {    // Screen params  };};
// Navigationnavigation.navigate('Details', {  // Navigation params});
```

GitHubAsk for support

Shared Transitions - FeedbackShare Your ThoughtsI value a lot your feedback! Help me improve by sharing your thoughts, suggestions, or reporting any issues you encounter. If you need assistance, send me an email at hello@reactiive.ioSend Feedback

---

*Documentation extracted from reactiive.io/demos*
