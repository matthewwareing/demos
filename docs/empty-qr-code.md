# Empty QR Code

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/empty-qr-code)
> **Source Code**: [/src/animations/empty-qr-code](/src/animations/empty-qr-code)

## Tags
- `skia`

## What's This About?

Empty Qr Code - FeedbackShare Your ThoughtsI value a lot your feedback! Help me improve by sharing your thoughts, suggestions, or reporting any issues you encounter. If you need assistance, send me an email at hello@reactiive.ioSend Feedback

## Technical Implementation

The component uses:

- QR code generation
- Ref-based toggle control
- Pressable scale animations
- Memoization for performance
- Custom share sheet

## Usage

```tsx
type QRCodeShareProps = {  qrCodeValue: string;};
// Basic usage<EmptyQRCode />;
// Custom implementationconst qrCodeShareRef = useRef<QRCodeShareRefType>(null);
<PressableScale  onPress={() => {    qrCodeShareRef.current?.toggle();  }}>  <QRCodeShare ref={qrCodeShareRef} qrCodeValue="https://example.com" /></PressableScale>;
```

GitHubAsk for support

Empty Qr Code - FeedbackShare Your ThoughtsI value a lot your feedback! Help me improve by sharing your thoughts, suggestions, or reporting any issues you encounter. If you need assistance, send me an email at hello@reactiive.ioSend Feedback

---

*Documentation extracted from reactiive.io/demos*
