# Threads Holo Ticket

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/threads-holo-ticket)
> **Source Code**: [/src/animations/threads-holo-ticket](/src/animations/threads-holo-ticket)

## Tags
- `reanimated`
- `gesture-handler`
- `skia`
- `react-native`

## Description

Scan to try on your device

## Features

- Interactive 3D flippable ticket with smooth animations
- Stunning holographic card effect with dynamic gradient patterns
- Gesture-based interaction (pan and tap)
- QR code on the back side with gradient fill (using react-native-qrcode-skia)
- Built with TypeScript for type safety

## Project Structure

```typescript
src/├── components/│   ├── ticket/│   │   ├── front-side.tsx  # Front side of the ticket with event details│   │   ├── back-side.tsx   # Back side with QR code│   │   └── index.tsx       # Main ticket component with flip animation│   └── holographic-card.tsx # Holographic effect using Skia└── index.tsx               # App entry point
```

## Usage

```tsx
import { Ticket } from './components/ticket';import { FrontSide } from './components/ticket/front-side';import { BackSide } from './components/ticket/back-side';
const App = () => {  return (    <View style={styles.container}>      <Ticket        width={300}        height={400}        frontSide={<FrontSide />}        backSide={<BackSide />}      />    </View>  );};
```

### Props

- width: Width of the ticket in pixels
- height: Height of the ticket in pixels
- frontSide: React component to render on the front of the ticket
- backSide: React component to render on the back of the ticket

### Interactions

- Pan: Swipe horizontally to rotate the ticket
- Tap: Tap to snap the ticket to the nearest complete rotation
- Holographic Effect: The holographic pattern responds to the ticket's rotation

---

*Documentation extracted from reactiive.io/demos*
