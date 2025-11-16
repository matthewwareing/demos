# Verification Code

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/verification-code)
> **Source Code**: [/src/animations/verification-code](/src/animations/verification-code)

## Tags
- `reanimated`
- `gesture-handler`

## What's This About?

This component creates an interactive verification code input screen with validation and feedback animations. It features a customizable code length, validation against a correct code, and visual feedback for user input. The implementation includes digit input handling, validation logic, and animated transitions, making it perfect for authentication flows or any scenario requiring secure code verification.

## Technical Implementation

The component uses:

- Code validation
- Input handling
- Visual feedback
- Animated transitions
- State management

## Usage

```tsx
// Basic usage with correct code<VerificationCode correctCode={31415} />
// Verification code screen<VerificationCodeScreen  correctCode={correctCode}  onSuccess={() => {    // Handle successful verification  }}  onError={() => {    // Handle verification error  }}/>
// Code validationconst validateCode = (input: string) => {  return input === String(correctCode);};
// Input handlingconst handleCodeChange = (code: string) => {  if (code.length === CODE_LENGTH) {    const isValid = validateCode(code);    if (isValid) {      onSuccess?.();    } else {      onError?.();    }  }};
// Animated feedbackconst animatedStyle = useAnimatedStyle(() => ({  transform: [    {      translateX: withSpring(isError.value ? 10 : 0, {        damping: 3,        stiffness: 100      })    }  ]}));
```

GitHubAsk for support

Verification Code - FeedbackShare Your ThoughtsI value a lot your feedback! Help me improve by sharing your thoughts, suggestions, or reporting any issues you encounter. If you need assistance, send me an email at hello@reactiive.ioSend Feedback

---

*Documentation extracted from reactiive.io/demos*
