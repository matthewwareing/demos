# Shake to Delete

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/shake-to-delete)
> **Source Code**: [/src/animations/shake-to-delete](/src/animations/shake-to-delete)

## Tags
- `reanimated`

## Description

Scan to try on your device

## Usage

```tsx
import { useShakingAnimation } from './hooks/use-shaking-animation';import { useIsShaking } from './hooks/use-is-shaking';
const MyComponent = () => {  // Get shaking controls  const { isShaking, toggleShaking, stopShaking } = useIsShaking();
  // Get shaking animation style for a specific item  const { rShakingStyle } = useShakingAnimation(1); // Unique ID for consistent animation
  return (    <Pressable onPress={stopShaking}>      <Animated.View style={[styles.container, rShakingStyle]}>        <TouchableOpacity onLongPress={toggleShaking} onPress={handlePress}>          {/* Your content */}        </TouchableOpacity>      </Animated.View>    </Pressable>  );};
```

### Animation Parameters

```tsx
export const SHAKING_ANIMATION = {  BASE: {    AMPLITUDE: 1, // Base shake distance    AMPLITUDE_VARIATION: 0.2,    DURATION: 80, // Base animation duration (ms)    DURATION_VARIATION: 40,    ROTATION_AMPLITUDE: 1, // Base rotation angle    ROTATION_VARIATION: 2,    ROTATION_BASE: -3,    ROTATION_BASE_VARIATION: 6,  },} as const;
```

---

*Documentation extracted from reactiive.io/demos*
