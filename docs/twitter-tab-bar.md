# Twitter Tab Bar

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/twitter-tab-bar)
> **Source Code**: [/src/animations/twitter-tab-bar](/src/animations/twitter-tab-bar)

## Tags
- `reanimated`

## Description

Scan to try on your device

## Technical Implementation

- Navigation system
- Context management
- Theme integration
- Custom tab bar
- Screen mapping

## Usage

```typescript
// Basic usage<TwitterTabBar />
// Full implementation with context<NavigationContainer theme={AppTheme}>  <ActiveTabBarContextProvider>    <BottomTab.Navigator      tabBar={(props) => (        <BottomTabBar {...props} />      )}    >      {screens.map(screen => (        <BottomTab.Screen          key={screen}          name={screen}          component={ScreenMap[screen]}        />      ))}    </BottomTab.Navigator>  </ActiveTabBarContextProvider></NavigationContainer>
// Theme configurationconst AppTheme = {  colors: {    background: Palette.background,    text: Palette.text,    border: Palette.text,    card: Palette.card  }};
// Screen mappingconst ScreenMap = {  Home: HomeScreen,  Search: SearchScreen,  Notifications: NotificationsScreen,  Message: MessageScreen};
// Screen namesconst ScreenNames = {  Home: 'Home',  Search: 'Search',  Notifications: 'Notifications',  Message: 'Message'};
```

---

*Documentation extracted from reactiive.io/demos*
