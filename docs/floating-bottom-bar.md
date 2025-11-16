# Floating Bottom Bar

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/floating-bottom-bar)
> **Source Code**: [/src/animations/floating-bottom-bar](/src/animations/floating-bottom-bar)

## Tags
- `reanimated`
- `skia`

## Description

Scan to try on your device

## What's This About?

- Floats above screen content
- Shows tab icons
- Handles navigation
- Uses custom tab bar
- Supports multiple screens

## Usage

```typescript
// Basic usage<FloatingBottomBar />;
// Navigation setupconst BottomTab = createBottomTabNavigator();
<BottomTab.Navigator tabBar={(props) => <BottomTabBar {...props} />}>  <BottomTab.Screen name="Home" component={HomeScreen} />  <BottomTab.Screen name="Bookmark" component={BookmarkScreen} />  <BottomTab.Screen name="Add" component={AddScreen} />  <BottomTab.Screen name="Profile" component={ProfileScreen} />  <BottomTab.Screen name="Settings" component={SettingsScreen} /></BottomTab.Navigator>;
```

---

*Documentation extracted from reactiive.io/demos*
