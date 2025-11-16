# Cuberto Slider

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/cuberto-slider)
> **Source Code**: [/src/animations/cuberto-slider](/src/animations/cuberto-slider)

## Tags
- `reanimated`
- `gesture-handler`

## Description

Scan to try on your device

## Technical Implementation

- Gesture-based interactions
- Smooth value transitions
- Custom styling and theming
- Performance optimizations with React.memo
- Responsive layout adaptations

## Usage

```typescript
// Basic usage with default settings<CubertoSlider />
// Custom implementation<Slider  min={0}  max={100}  step={1}  onValueChange={(value) => {    console.log('Current value:', value);  }}/>
// With gesture handler root<GestureHandlerRootView>  <CubertoSlider /></GestureHandlerRootView>
```

---

*Documentation extracted from reactiive.io/demos*
