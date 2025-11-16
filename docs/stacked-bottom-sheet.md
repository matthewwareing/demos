# Stacked Bottom Sheet

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/stacked-bottom-sheet)
> **Source Code**: [/src/animations/stacked-bottom-sheet](/src/animations/stacked-bottom-sheet)

## Tags
- `reanimated`
- `gesture-handler`

## Description

Scan to try on your device

## Technical Implementation

- Sheet management
- Gesture handling
- Safe area awareness
- Provider pattern
- Stack navigation

## Usage

```typescript
// Basic usage with provider<StackedBottomSheet />
// Full implementation<SafeAreaProvider>  <GestureHandlerRootView style={{ flex: 1 }}>    <StackedSheetProvider>      <App />    </StackedSheetProvider>  </GestureHandlerRootView></SafeAreaProvider>
// Trigger sheetconst { onPress } = useDemoStackedSheet();
// Action button<PressableScale  style={styles.button}  onPress={onPress}>  <Text style={styles.textButton}>    Show Action Tray  </Text></PressableScale>
// Stylingconst styles = StyleSheet.create({  button: {    paddingVertical: 18,    paddingHorizontal: 25,    backgroundColor: '#111',    borderRadius: 25,    borderWidth: 1  },  textButton: {    color: 'white',    letterSpacing: 1.2,    textTransform: 'uppercase',    fontWeight: '700'  }});
```

---

*Documentation extracted from reactiive.io/demos*
