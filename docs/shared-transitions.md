# Shared Transitions

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/shared-transitions)
> **Source Code**: [/src/animations/shared-transitions](/src/animations/shared-transitions)

## Tags
- `reanimated`

## Description

Scan to try on your device

## Technical Implementation

- React Navigation
- Stack navigation
- Shared elements
- Custom animations
- Screen transitions

## Usage

```typescript
// Navigation setupconst Stack = createNativeStackNavigator<RootStackParamsList>();
// Basic usage<Stack.Navigator  initialRouteName="Home"  screenOptions={{    animation: 'fade',    animationDuration: 300,  }}>  <Stack.Screen name="Home" component={HomeScreen} />  <Stack.Screen name="Details" component={DetailsScreen} /></Stack.Navigator>;
// Screen typestype RootStackParamsList = {  Home: undefined;  Details: {    // Screen params  };};
// Navigationnavigation.navigate('Details', {  // Navigation params});
```

---

*Documentation extracted from reactiive.io/demos*
