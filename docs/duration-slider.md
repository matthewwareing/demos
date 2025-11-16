# Duration Slider

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/duration-slider)
> **Source Code**: [/src/animations/duration-slider](/src/animations/duration-slider)

## Tags
- `skia`

## What's This About?

Duration Slider - FeedbackShare Your ThoughtsI value a lot your feedback! Help me improve by sharing your thoughts, suggestions, or reporting any issues you encounter. If you need assistance, send me an email at hello@reactiive.ioSend Feedback

## Technical Implementation

The component uses:

- Skia for rendering
- Custom font loading
- Responsive sizing
- Value range management
- Rotation gesture handling

## Usage

```tsx
type CircularSliderProps = {  minVal: number;  maxVal: number;  width: number;  height: number;  font: SkFont;  onValueChange: (value: number) => void;};
// Basic usageconst font = useFont(sfProRoundedBold, 100);
{  font && (    <CircularSlider      minVal={1}      maxVal={12}      width={300}      height={300}      font={font}      onValueChange={(value) => {        console.log('Selected duration:', value);      }}    />  );}
```

GitHubAsk for support

Duration Slider - FeedbackShare Your ThoughtsI value a lot your feedback! Help me improve by sharing your thoughts, suggestions, or reporting any issues you encounter. If you need assistance, send me an email at hello@reactiive.ioSend Feedback

---

*Documentation extracted from reactiive.io/demos*
