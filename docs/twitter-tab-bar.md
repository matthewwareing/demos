# Twitter Tab Bar

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/twitter-tab-bar)
> **Source Code**: [/src/animations/twitter-tab-bar](/src/animations/twitter-tab-bar)

## Tags
- `reanimated`

## What's This About?

This component recreates Twitter's bottom tab navigation system with smooth transitions and animations. It features a custom tab bar implementation with context-based active tab management and theme integration. The implementation includes screen navigation, custom styling, and animated tab indicators, making it perfect for applications requiring a polished, Twitter-like navigation experience.

## Technical Implementation

The component uses:

- Navigation system
- Context management
- Theme integration
- Custom tab bar
- Screen mapping

## Usage

```tsx
// Basic usage<TwitterTabBar />
// Full implementation with context<NavigationContainer theme={AppTheme}>  <ActiveTabBarContextProvider>    <BottomTab.Navigator      tabBar={(props) => (        <BottomTabBar {...props} />      )}    >      {screens.map(screen => (        <BottomTab.Screen          key={screen}          name={screen}          component={ScreenMap[screen]}        />      ))}    </BottomTab.Navigator>  </ActiveTabBarContextProvider></NavigationContainer>
// Theme configurationconst AppTheme = {  colors: {    background: Palette.background,    text: Palette.text,    border: Palette.text,    card: Palette.card  }};
// Screen mappingconst ScreenMap = {  Home: HomeScreen,  Search: SearchScreen,  Notifications: NotificationsScreen,  Message: MessageScreen};
// Screen namesconst ScreenNames = {  Home: 'Home',  Search: 'Search',  Notifications: 'Notifications',  Message: 'Message'};
```

GitHubAsk for support

Twitter Tab Bar - FeedbackShare Your ThoughtsI value a lot your feedback! Help me improve by sharing your thoughts, suggestions, or reporting any issues you encounter. If you need assistance, send me an email at hello@reactiive.ioSend Feedback

---

*Documentation extracted from reactiive.io/demos*
