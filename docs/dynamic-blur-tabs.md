# Dynamic Blur Tabs

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/dynamic-blur-tabs)
> **Source Code**: [/src/animations/dynamic-blur-tabs](/src/animations/dynamic-blur-tabs)

## Tags
- `reanimated`
- `expo-blur`

## What's This About?

Dynamic Blur Tabs - FeedbackShare Your ThoughtsI value a lot your feedback! Help me improve by sharing your thoughts, suggestions, or reporting any issues you encounter. If you need assistance, send me an email at hello@reactiive.ioSend Feedback

## Technical Implementation

The component uses:

- React Navigation's bottom tabs
- Custom tab bar component
- Screen freezing for performance
- Dynamic screen mapping
- Gradient backgrounds

## Usage

```tsx
// Basic usage<DynamicBlurTabs />;
// Component structureconst BottomTab = createBottomTabNavigator();
<BottomTab.Navigator  initialRouteName="home"  screenOptions={{    headerShown: false,  }}  tabBar={(props) => <BottomTabBar {...props} />}>  {screens.map((screen) => (    <BottomTab.Screen      key={screen.name}      name={screen.name}      component={screen.component}      options={{ freezeOnBlur: true }}    />  ))}</BottomTab.Navigator>;
```

GitHubAsk for support

Dynamic Blur Tabs - FeedbackShare Your ThoughtsI value a lot your feedback! Help me improve by sharing your thoughts, suggestions, or reporting any issues you encounter. If you need assistance, send me an email at hello@reactiive.ioSend Feedback

---

*Documentation extracted from reactiive.io/demos*
