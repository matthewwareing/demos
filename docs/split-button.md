# Split Button

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/split-button)
> **Source Code**: [/src/animations/split-button](/src/animations/split-button)

## Tags
- `reanimated`
- `gesture-handler`

## What's This About?

This component creates an interactive split button that can display different icons on each side. It features gesture handling for smooth interactions and supports custom icon integration from Expo's vector icons library. The implementation is perfect for social login buttons, toggle switches, or any interface requiring a dual-state button.

## Technical Implementation

The component uses:

- Gesture handling
- Icon integration
- Split states
- Custom styling
- Touch feedback

## Usage

```tsx
// Basic usage<SplitButton />
// With custom icons<SplitButton  rightIcon={    <AntDesign      name="apple1"      size={21}      color={colors.background}    />  }  leftIcon={    <AntDesign      name="google"      size={22}      color={colors.almostBlack}    />  }/>
// Full implementation<GestureHandlerRootView style={{ flex: 1 }}>  <View style={styles.container}>    <SplitButton      rightIcon={rightIcon}      leftIcon={leftIcon}    />  </View></GestureHandlerRootView>
// Color themingconst colors = {  background: '#FFFFFF',  almostBlack: '#1A1A1A'};
```

GitHubAsk for support

Split Button - FeedbackShare Your ThoughtsI value a lot your feedback! Help me improve by sharing your thoughts, suggestions, or reporting any issues you encounter. If you need assistance, send me an email at hello@reactiive.ioSend Feedback

---

*Documentation extracted from reactiive.io/demos*
