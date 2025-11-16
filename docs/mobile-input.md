# Mobile Input

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/mobile-input)
> **Source Code**: [/src/animations/mobile-input](/src/animations/mobile-input)

## Tags
- `reanimated`
- `skia`

## Description

Scan to try on your device

## Technical Implementation

- PIN validation
- Error handling
- Input clearing
- Completion events
- Visual feedback

## Usage

```typescript
// Basic usage with callbacks<LockScreen  correctPin="11111"  onError={(wrongPin) => {    console.log('Wrong PIN entered:', wrongPin);  }}  onClear={() => {    console.log('PIN cleared');  }}  onCompleted={() => {    console.log('Correct PIN entered');  }}/>;
// Component propstype LockScreenProps = {  correctPin: string;  onError: (wrongPin: string) => void;  onClear: () => void;  onCompleted: () => void;};
```

---

*Documentation extracted from reactiive.io/demos*
