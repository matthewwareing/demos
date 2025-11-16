# Stacked Bottom Sheet

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/stacked-bottom-sheet)
> **Source Code**: [/src/animations/stacked-bottom-sheet](/src/animations/stacked-bottom-sheet)

## Tags
- `reanimated`
- `gesture-handler`

## What's This About?

This component creates a sophisticated bottom sheet system that can manage multiple stacked sheets. It features a provider-based architecture for sheet management, safe area handling, and gesture controls. The implementation includes smooth animations and transitions between sheets, making it perfect for complex modal interfaces requiring multiple layers of interaction.

## Technical Implementation

The component uses:

- Sheet management
- Gesture handling
- Safe area awareness
- Provider pattern
- Stack navigation

## Usage

```tsx
// Basic usage with provider<StackedBottomSheet />
// Full implementation<SafeAreaProvider>  <GestureHandlerRootView style={{ flex: 1 }}>    <StackedSheetProvider>      <App />    </StackedSheetProvider>  </GestureHandlerRootView></SafeAreaProvider>
// Trigger sheetconst { onPress } = useDemoStackedSheet();
// Action button<PressableScale  style={styles.button}  onPress={onPress}>  <Text style={styles.textButton}>    Show Action Tray  </Text></PressableScale>
// Stylingconst styles = StyleSheet.create({  button: {    paddingVertical: 18,    paddingHorizontal: 25,    backgroundColor: '#111',    borderRadius: 25,    borderWidth: 1  },  textButton: {    color: 'white',    letterSpacing: 1.2,    textTransform: 'uppercase',    fontWeight: '700'  }});
```

GitHubAsk for support

Stacked Bottom Sheet - FeedbackShare Your ThoughtsI value a lot your feedback! Help me improve by sharing your thoughts, suggestions, or reporting any issues you encounter. If you need assistance, send me an email at hello@reactiive.ioSend Feedback

---

*Documentation extracted from reactiive.io/demos*
