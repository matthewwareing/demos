# BottomBarSkia

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/bottom-bar-skia)
> **Source Code**: [/src/animations/bottom-bar-skia](/src/animations/bottom-bar-skia)

## Tags
- `skia`

## Description

Scan to try on your device

## Technical Implementation

- Custom tab bar implementation with Skia
- Seamless integration with React Navigation
- Optimized performance through hardware acceleration
- Support for standard navigation patterns

## Usage

```typescript
// Setup the navigatorconst BottomTab = createBottomTabNavigator();
// Basic usage<BottomBarSkia />
// Full configuration<BottomTab.Navigator  tabBar={props => <BottomTabBar {...props} />}>  <BottomTab.Screen    name="Home"    component={HomeScreen}  />  <BottomTab.Screen    name="Search"    component={SearchScreen}  />  <BottomTab.Screen    name="User"    component={UserScreen}  /></BottomTab.Navigator>
```

---

*Documentation extracted from reactiive.io/demos*
