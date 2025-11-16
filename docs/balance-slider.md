# Balance Slider

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/balance-slider)
> **Source Code**: [/src/animations/balance-slider](/src/animations/balance-slider)

## Tags
- `reanimated`
- `gesture-handler`

## Description

Scan to try on your device

## Usage

```typescript
type BalanceSliderProps = {  width: number;  height: number;  onChange: (values: {    leftPercentage: number;    rightPercentage: number;  }) => void;  leftLabel: string;  rightLabel: string;  colors: {    left: {      box: string;      label: string;      percentage: string;    };    right: {      box: string;      label: string;      percentage: string;    };  };  leftPercentageLimitBeforeShift: number;  rightPercentageLimitBeforeShift: number;};
// Example usage<BalanceSlider  width={300}  height={50}  leftLabel="Coffee"  rightLabel="Milk"  onChange={({ leftPercentage, rightPercentage }) => {    console.log(leftPercentage, rightPercentage);  }}/>;
```

---

*Documentation extracted from reactiive.io/demos*
