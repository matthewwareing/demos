# Mobile Input

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/mobile-input)
> **Source Code**: [/src/animations/mobile-input](/src/animations/mobile-input)

## Tags
- `reanimated`
- `skia`

## What's This About?

This component creates a secure PIN input interface similar to mobile device lock screens. It handles PIN validation with animated feedback, providing visual cues for correct and incorrect entries. The component includes event callbacks for various states including errors, clearing, and successful completion, making it suitable for authentication workflows.

## Technical Implementation

The component uses:

- PIN validation
- Error handling
- Input clearing
- Completion events
- Visual feedback

## Usage

```tsx
// Basic usage with callbacks<LockScreen  correctPin="11111"  onError={(wrongPin) => {    console.log('Wrong PIN entered:', wrongPin);  }}  onClear={() => {    console.log('PIN cleared');  }}  onCompleted={() => {    console.log('Correct PIN entered');  }}/>;
// Component propstype LockScreenProps = {  correctPin: string;  onError: (wrongPin: string) => void;  onClear: () => void;  onCompleted: () => void;};
```

GitHubAsk for support

Mobile Input - FeedbackShare Your ThoughtsI value a lot your feedback! Help me improve by sharing your thoughts, suggestions, or reporting any issues you encounter. If you need assistance, send me an email at hello@reactiive.ioSend Feedback

---

*Documentation extracted from reactiive.io/demos*
