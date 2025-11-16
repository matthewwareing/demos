# Particles Button

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/particles-button)
> **Source Code**: [/src/animations/particles-button](/src/animations/particles-button)

## Tags
- `reanimated`
- `gesture-handler`
- `skia`

## Description

Scan to try on your device

## Usage

```tsx
import { CircularButton } from 'sparks-button';
const App = () => {  return (    <CircularButton      size={48}      blastRadius={48}      onPress={() => {        console.log('Button pressed!');      }}    />  );};
```

## Props

```typescript
type CircularButtonProps = {  size: number; // Size of the circular button  blastRadius: number; // Radius of the blast effect animation  baseIcon?: React.ReactNode; // Custom icon for the base state (defaults to Plus icon)  activeIcon?: React.ReactNode; // Custom icon for the active state (defaults to Check icon)  autoReset?: boolean; // Whether to automatically reset the button state after animation (defaults to true)  onPress?: () => void; // Callback function called when the button is pressed};
```

---

*Documentation extracted from reactiive.io/demos*
