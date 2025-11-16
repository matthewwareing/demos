# Telegram Theme Switch

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/telegram-theme-switch)
> **Source Code**: [/src/animations/telegram-theme-switch](/src/animations/telegram-theme-switch)

## Tags
- `reanimated`
- `gesture-handler`
- `skia`

## What's This About?

This component creates a theme switching system similar to Telegram's interface, featuring a bottom tab navigation and smooth theme transitions. It includes a provider-based theme management system, customizable color palettes for light and dark themes, and integration with React Navigation. The implementation is perfect for applications requiring sophisticated theme switching capabilities with bottom tab navigation.

## Technical Implementation

The component uses:

- Theme management
- Navigation system
- Color palettes
- Provider pattern
- Safe area handling

## Usage

```tsx
// Basic usage<TelegramThemeSwitch />
// Full implementation with provider<SwitchThemeProvider>  <NavigationContainer theme={selectedTheme}>    <SafeAreaProvider>      <TelegramThemeSwitch />    </SafeAreaProvider>  </NavigationContainer></SwitchThemeProvider>
// Theme configurationconst LightTheme = {  colors: {    background: LightPalette.background,    text: LightPalette.text,    border: LightPalette.text,    card: LightPalette.card  }};
const DarkTheme = {  colors: {    background: DarkPalette.background,    text: DarkPalette.text,    border: DarkPalette.text,    card: DarkPalette.card  }};
// Theme hook usageconst { theme } = useSwitchTheme();const selectedTheme = theme === 'light' ?  LightTheme :  DarkTheme;
// Navigation setup<BottomTab.Navigator  initialRouteName="Search"  tabBar={(props) => (    <BottomTabBar {...props} />  )}>  {screens.map(screen => (    <BottomTab.Screen      key={screen}      name={screen}      component={ScreenMap[screen]}    />  ))}</BottomTab.Navigator>
```

GitHubAsk for support

Telegram Theme Switch - FeedbackShare Your ThoughtsI value a lot your feedback! Help me improve by sharing your thoughts, suggestions, or reporting any issues you encounter. If you need assistance, send me an email at hello@reactiive.ioSend Feedback

---

*Documentation extracted from reactiive.io/demos*
