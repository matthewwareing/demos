# BottomBarSkia

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/bottom-bar-skia)
> **Source Code**: [/src/animations/bottom-bar-skia](/src/animations/bottom-bar-skia)

## Tags
- `skia`

## What's This About?

This component implements a bottom navigation bar using Skia for rendering, providing butter-smooth animations and transitions. It integrates seamlessly with React Navigation's bottom tab navigator while offering enhanced visual effects and performance.

## Technical Implementation

The component leverages Skia for rendering and React Navigation for routing:

- Custom tab bar implementation with Skia
- Seamless integration with React Navigation
- Optimized performance through hardware acceleration
- Support for standard navigation patterns

## Usage

```tsx
// Setup the navigatorconst BottomTab = createBottomTabNavigator();
// Basic usage<BottomBarSkia />
// Full configuration<BottomTab.Navigator  tabBar={props => <BottomTabBar {...props} />}>  <BottomTab.Screen    name="Home"    component={HomeScreen}  />  <BottomTab.Screen    name="Search"    component={SearchScreen}  />  <BottomTab.Screen    name="User"    component={UserScreen}  /></BottomTab.Navigator>
```

GitHubAsk for support

Bottom Bar Skia - FeedbackShare Your ThoughtsI value a lot your feedback! Help me improve by sharing your thoughts, suggestions, or reporting any issues you encounter. If you need assistance, send me an email at hello@reactiive.ioSend Feedback

---

*Documentation extracted from reactiive.io/demos*
