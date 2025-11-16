# Telegram Theme Switch

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/telegram-theme-switch)
> **Source Code**: [/src/animations/telegram-theme-switch](/src/animations/telegram-theme-switch)

## Tags
- `reanimated`
- `gesture-handler`
- `skia`

## Description

Scan to try on your device

## Technical Implementation

- Theme management
- Navigation system
- Color palettes
- Provider pattern
- Safe area handling

## Usage

```typescript
// Basic usage<TelegramThemeSwitch />
// Full implementation with provider<SwitchThemeProvider>  <NavigationContainer theme={selectedTheme}>    <SafeAreaProvider>      <TelegramThemeSwitch />    </SafeAreaProvider>  </NavigationContainer></SwitchThemeProvider>
// Theme configurationconst LightTheme = {  colors: {    background: LightPalette.background,    text: LightPalette.text,    border: LightPalette.text,    card: LightPalette.card  }};
const DarkTheme = {  colors: {    background: DarkPalette.background,    text: DarkPalette.text,    border: DarkPalette.text,    card: DarkPalette.card  }};
// Theme hook usageconst { theme } = useSwitchTheme();const selectedTheme = theme === 'light' ?  LightTheme :  DarkTheme;
// Navigation setup<BottomTab.Navigator  initialRouteName="Search"  tabBar={(props) => (    <BottomTabBar {...props} />  )}>  {screens.map(screen => (    <BottomTab.Screen      key={screen}      name={screen}      component={ScreenMap[screen]}    />  ))}</BottomTab.Navigator>
```

---

*Documentation extracted from reactiive.io/demos*
