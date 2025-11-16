# Staggered Card Number

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/staggered-card-number)
> **Source Code**: [/src/animations/staggered-card-number](/src/animations/staggered-card-number)

## Tags
- `reanimated`

## What's This About?

This component creates an animated display for credit card numbers with staggered reveal animations. Each digit appears with a coordinated timing sequence, creating a smooth and engaging reveal effect. The implementation is perfect for payment interfaces or any scenario where card numbers need to be displayed with visual flair.

## Technical Implementation

The component uses:

- Staggered animations
- Number formatting
- Card validation
- Coordinated timing
- Visual feedback

## Usage

```tsx
// Basic usage<StaggeredCardNumber />
// Card info component<CardInfo  cardNumber={2223000048400011}/>
// Stylingconst styles = StyleSheet.create({  container: {    flex: 1,    backgroundColor: '#eaeaea',    alignItems: 'center',    justifyContent: 'center'  }});
// Typestype CardInfoProps = {  cardNumber: number;  // Additional props for customization  format?: boolean;  animate?: boolean;  staggerDelay?: number;};
// Card number formattingconst formatCardNumber = (number: number) => {  return number.toString()    .replace(/(\d{4})/g, '$1 ')    .trim();};
```

GitHubAsk for support

Staggered Card Number - FeedbackShare Your ThoughtsI value a lot your feedback! Help me improve by sharing your thoughts, suggestions, or reporting any issues you encounter. If you need assistance, send me an email at hello@reactiive.ioSend Feedback

---

*Documentation extracted from reactiive.io/demos*
