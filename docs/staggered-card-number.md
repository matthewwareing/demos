# Staggered Card Number

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/staggered-card-number)
> **Source Code**: [/src/animations/staggered-card-number](/src/animations/staggered-card-number)

## Tags
- `reanimated`

## Description

Scan to try on your device

## Technical Implementation

- Staggered animations
- Number formatting
- Card validation
- Coordinated timing
- Visual feedback

## Usage

```typescript
// Basic usage<StaggeredCardNumber />
// Card info component<CardInfo  cardNumber={2223000048400011}/>
// Stylingconst styles = StyleSheet.create({  container: {    flex: 1,    backgroundColor: '#eaeaea',    alignItems: 'center',    justifyContent: 'center'  }});
// Typestype CardInfoProps = {  cardNumber: number;  // Additional props for customization  format?: boolean;  animate?: boolean;  staggerDelay?: number;};
// Card number formattingconst formatCardNumber = (number: number) => {  return number.toString()    .replace(/(\d{4})/g, '$1 ')    .trim();};
```

---

*Documentation extracted from reactiive.io/demos*
