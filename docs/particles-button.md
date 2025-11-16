# Particles Button

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/particles-button)
> **Source Code**: [/src/animations/particles-button](/src/animations/particles-button)

## Tags
- `reanimated`
- `gesture-handler`
- `skia`

## Usage

```tsx
import { CircularButton } from 'sparks-button';
const App = () => {  return (    <CircularButton      size={48}      blastRadius={48}      onPress={() => {        console.log('Button pressed!');      }}    />  );};
```

## Props

The CircularButton component accepts the following props:

```typescript
type CircularButtonProps = {  size: number; // Size of the circular button  blastRadius: number; // Radius of the blast effect animation  baseIcon?: React.ReactNode; // Custom icon for the base state (defaults to Plus icon)  activeIcon?: React.ReactNode; // Custom icon for the active state (defaults to Check icon)  autoReset?: boolean; // Whether to automatically reset the button state after animation (defaults to true)  onPress?: () => void; // Callback function called when the button is pressed};
```

GitHubAsk for support

Particles Button - FeedbackShare Your ThoughtsI value a lot your feedback! Help me improve by sharing your thoughts, suggestions, or reporting any issues you encounter. If you need assistance, send me an email at hello@reactiive.ioSend Feedback

---

*Documentation extracted from reactiive.io/demos*
