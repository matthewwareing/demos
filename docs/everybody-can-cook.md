# Everybody Can Cook

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/everybody-can-cook)
> **Source Code**: [/src/animations/everybody-can-cook](/src/animations/everybody-can-cook)

## Tags
- `reanimated`

## Description

Scan to try on your device

## Usage

```tsx
import { useRef } from 'react';import {  StaggeredText,  type StaggeredTextRef,} from './components/staggered-text';
const MyComponent = () => {  const textRef = useRef<StaggeredTextRef>(null);
  return (    <StaggeredText      text="Hello World"      ref={textRef}      fontSize={50}      delay={300}      // Optional: Enable reverse animation      // enableReverse={true}    />  );};
```

### Controlling the Animation

```typescript
// Start the animationtextRef.current?.animate();
// Reset to initial statetextRef.current?.reset();
// Toggle animation (requires enableReverse prop)textRef.current?.toggleAnimate();
```

---

*Documentation extracted from reactiive.io/demos*
