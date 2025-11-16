# Family Number Input

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/family-number-input)
> **Source Code**: [/src/animations/family-number-input](/src/animations/family-number-input)

## Tags
- `reanimated`
- `gesture-handler`

## Description

Scan to try on your device

## What's This About?

- Shows animated number changes
- Provides a button grid interface
- Handles input validation
- Includes reset functionality
- Uses gradient overlay effects

## Usage

```typescript
// Basic usage<FamilyNumberInput />
// Component structure<SafeAreaView>  <AnimatedNumber value={input} />  <ButtonsGrid    input={input}    onUpdate={(value) => setInput(value)}    onBackspace={(value) => setInput(value)}    onReset={() => setInput(0)}    onMaxReached={() => {      // Handle maximum value reached    }}  /></SafeAreaView>
```

---

*Documentation extracted from reactiive.io/demos*
