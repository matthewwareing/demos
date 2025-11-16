# Slide to Reveal

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/slide-to-reveal)
> **Source Code**: [/src/animations/slide-to-reveal](/src/animations/slide-to-reveal)

## Tags
- `gesture-handler`
- `skia`

## Description

Scan to try on your device

## Technical Implementation

- Gesture handling
- Screen adaptation
- Code revelation
- Size customization
- Interactive sliding

## Usage

```typescript
// Basic usage<SlideToReveal />
// With custom dimensions and code<SlideToReveal  code={112358}  width={windowWidth * 0.6}  height={80}/>
// Full implementation<GestureHandlerRootView style={{ flex: 1 }}>  <View style={styles.container}>    <SlideToReveal      code={112358}      width={windowWidth * 0.6}      height={80}    />  </View></GestureHandlerRootView>
// Window dimensionsconst { width: windowWidth } = useWindowDimensions();
```

---

*Documentation extracted from reactiive.io/demos*
