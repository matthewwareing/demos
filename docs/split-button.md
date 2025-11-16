# Split Button

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/split-button)
> **Source Code**: [/src/animations/split-button](/src/animations/split-button)

## Tags
- `reanimated`
- `gesture-handler`

## Description

Scan to try on your device

## Technical Implementation

- Gesture handling
- Icon integration
- Split states
- Custom styling
- Touch feedback

## Usage

```typescript
// Basic usage<SplitButton />
// With custom icons<SplitButton  rightIcon={    <AntDesign      name="apple1"      size={21}      color={colors.background}    />  }  leftIcon={    <AntDesign      name="google"      size={22}      color={colors.almostBlack}    />  }/>
// Full implementation<GestureHandlerRootView style={{ flex: 1 }}>  <View style={styles.container}>    <SplitButton      rightIcon={rightIcon}      leftIcon={leftIcon}    />  </View></GestureHandlerRootView>
// Color themingconst colors = {  background: '#FFFFFF',  almostBlack: '#1A1A1A'};
```

---

*Documentation extracted from reactiive.io/demos*
