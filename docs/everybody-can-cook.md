# Everybody Can Cook

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/everybody-can-cook)
> **Source Code**: [/src/animations/everybody-can-cook](/src/animations/everybody-can-cook)

## Tags
- `reanimated`

## Usage

The main component StaggeredText can be used to create animated text:

```tsx
import { useRef } from 'react';import {  StaggeredText,  type StaggeredTextRef,} from './components/staggered-text';
const MyComponent = () => {  const textRef = useRef<StaggeredTextRef>(null);
  return (    <StaggeredText      text="Hello World"      ref={textRef}      fontSize={50}      delay={300}      // Optional: Enable reverse animation      // enableReverse={true}    />  );};
```

### Controlling the Animation

The component exposes three methods through its ref:

```typescript
// Start the animationtextRef.current?.animate();
// Reset to initial statetextRef.current?.reset();
// Toggle animation (requires enableReverse prop)textRef.current?.toggleAnimate();
```

GitHubAsk for support

Everybody Can Cook - FeedbackShare Your ThoughtsI value a lot your feedback! Help me improve by sharing your thoughts, suggestions, or reporting any issues you encounter. If you need assistance, send me an email at hello@reactiive.ioSend Feedback

---

*Documentation extracted from reactiive.io/demos*
