# Duration Slider

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/duration-slider)
> **Source Code**: [/src/animations/duration-slider](/src/animations/duration-slider)

## Tags
- `skia`

## Description

Scan to try on your device

## What's This About?

- Shows duration values from 1 to 12
- Updates value through rotation
- Uses custom SF Pro Rounded font
- Adapts to screen width

## Technical Implementation

- Skia for rendering
- Custom font loading
- Responsive sizing
- Value range management
- Rotation gesture handling

## Usage

```typescript
type CircularSliderProps = {  minVal: number;  maxVal: number;  width: number;  height: number;  font: SkFont;  onValueChange: (value: number) => void;};
// Basic usageconst font = useFont(sfProRoundedBold, 100);
{  font && (    <CircularSlider      minVal={1}      maxVal={12}      width={300}      height={300}      font={font}      onValueChange={(value) => {        console.log('Selected duration:', value);      }}    />  );}
```

---

*Documentation extracted from reactiive.io/demos*
