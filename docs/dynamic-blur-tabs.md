# Dynamic Blur Tabs

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/dynamic-blur-tabs)
> **Source Code**: [/src/animations/dynamic-blur-tabs](/src/animations/dynamic-blur-tabs)

## Tags
- `reanimated`
- `expo-blur`

## Description

Scan to try on your device

## What's This About?

- Shows blur effects while scrolling
- Uses React Navigation for routing
- Supports multiple screens
- Freezes inactive screens

## Technical Implementation

- React Navigation's bottom tabs
- Custom tab bar component
- Screen freezing for performance
- Dynamic screen mapping
- Gradient backgrounds

## Usage

```typescript
// Basic usage<DynamicBlurTabs />;
// Component structureconst BottomTab = createBottomTabNavigator();
<BottomTab.Navigator  initialRouteName="home"  screenOptions={{    headerShown: false,  }}  tabBar={(props) => <BottomTabBar {...props} />}>  {screens.map((screen) => (    <BottomTab.Screen      key={screen.name}      name={screen.name}      component={screen.component}      options={{ freezeOnBlur: true }}    />  ))}</BottomTab.Navigator>;
```

---

*Documentation extracted from reactiive.io/demos*
