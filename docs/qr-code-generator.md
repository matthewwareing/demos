# QR Code Generator

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/qr-code-generator)
> **Source Code**: [/src/animations/qr-code-generator](/src/animations/qr-code-generator)

## Tags
- `skia`

## Description

Scan to try on your device

## Technical Implementation

- Skia rendering
- Gradient effects
- Path manipulation
- Text input handling
- Interactive sliders

## Usage

```typescript
// Basic usage<QRCodeGenerator />
// QR code with effects<QRCode  value="reactiive.io"  size={windowWidth * 0.9}  strokeWidth={strokeWidthProgress}  errorCorrectionLevel="H">  <SweepGradient    c={vec(windowWidth / 2, windowWidth / 2)}    colors={['cyan', 'magenta', 'cyan']}  />  <DiscretePathEffect    length={10}    deviation={deviationProgress}  /></QRCode>
// Slider for adjusting effects<Slider  initialProgress={0.5}  maxValue={6}  onUpdate={(progress) => {    deviationProgress.value = progress;  }}/>
```

---

*Documentation extracted from reactiive.io/demos*
