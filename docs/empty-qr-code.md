# Empty QR Code

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/empty-qr-code)
> **Source Code**: [/src/animations/empty-qr-code](/src/animations/empty-qr-code)

## Tags
- `skia`

## Description

Scan to try on your device

## What's This About?

- Shows/hides with animation
- Includes share functionality
- Uses pressable scale feedback
- Handles QR code generation

## Technical Implementation

- QR code generation
- Ref-based toggle control
- Pressable scale animations
- Memoization for performance
- Custom share sheet

## Usage

```typescript
type QRCodeShareProps = {  qrCodeValue: string;};
// Basic usage<EmptyQRCode />;
// Custom implementationconst qrCodeShareRef = useRef<QRCodeShareRefType>(null);
<PressableScale  onPress={() => {    qrCodeShareRef.current?.toggle();  }}>  <QRCodeShare ref={qrCodeShareRef} qrCodeValue="https://example.com" /></PressableScale>;
```

---

*Documentation extracted from reactiive.io/demos*
