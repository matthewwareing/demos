# Verification Code

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/verification-code)
> **Source Code**: [/src/animations/verification-code](/src/animations/verification-code)

## Tags
- `reanimated`
- `gesture-handler`

## Description

Scan to try on your device

## Technical Implementation

- Code validation
- Input handling
- Visual feedback
- Animated transitions
- State management

## Usage

```typescript
// Basic usage with correct code<VerificationCode correctCode={31415} />
// Verification code screen<VerificationCodeScreen  correctCode={correctCode}  onSuccess={() => {    // Handle successful verification  }}  onError={() => {    // Handle verification error  }}/>
// Code validationconst validateCode = (input: string) => {  return input === String(correctCode);};
// Input handlingconst handleCodeChange = (code: string) => {  if (code.length === CODE_LENGTH) {    const isValid = validateCode(code);    if (isValid) {      onSuccess?.();    } else {      onError?.();    }  }};
// Animated feedbackconst animatedStyle = useAnimatedStyle(() => ({  transform: [    {      translateX: withSpring(isError.value ? 10 : 0, {        damping: 3,        stiffness: 100      })    }  ]}));
```

---

*Documentation extracted from reactiive.io/demos*
