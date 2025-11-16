# QR Code Generator

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/qr-code-generator)
> **Source Code**: [/src/animations/qr-code-generator](/src/animations/qr-code-generator)

## Tags
- `skia`

## What's This About?

This component creates a dynamic QR code generator with customizable visual effects. Users can input text to generate QR codes that feature gradient colors and adjustable path effects. The implementation includes interactive sliders for controlling visual parameters like deviation and stroke width, making it possible to create unique and visually appealing QR codes.

## Technical Implementation

The component uses:

- Skia rendering
- Gradient effects
- Path manipulation
- Text input handling
- Interactive sliders

## Usage

```tsx
// Basic usage<QRCodeGenerator />
// QR code with effects<QRCode  value="reactiive.io"  size={windowWidth * 0.9}  strokeWidth={strokeWidthProgress}  errorCorrectionLevel="H">  <SweepGradient    c={vec(windowWidth / 2, windowWidth / 2)}    colors={['cyan', 'magenta', 'cyan']}  />  <DiscretePathEffect    length={10}    deviation={deviationProgress}  /></QRCode>
// Slider for adjusting effects<Slider  initialProgress={0.5}  maxValue={6}  onUpdate={(progress) => {    deviationProgress.value = progress;  }}/>
```

GitHubAsk for support

Qr Code Generator - FeedbackShare Your ThoughtsI value a lot your feedback! Help me improve by sharing your thoughts, suggestions, or reporting any issues you encounter. If you need assistance, send me an email at hello@reactiive.ioSend Feedback

---

*Documentation extracted from reactiive.io/demos*
