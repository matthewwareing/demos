# Action Tray

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/action-tray)
> **Source Code**: [/src/animations/action-tray](/src/animations/action-tray)

## Tags
- `reanimated`
- `gesture-handler`
- `react-native`

## What's This About?

The Action Tray creates a bottom sheet interface that:

## How It Works

The component is built with two main parts:

- ActionTray: The core component that:Handles gesture interactionsManages the sliding animationControls the tray's positionProvides imperative methods for programmatic control
- Handles gesture interactions
- Manages the sliding animation
- Controls the tray's position
- Provides imperative methods for programmatic control
- Main Interface: A demonstration that showcases:Multiple content statesDynamic height adjustmentsSmooth transitions between statesA toggle button with rotation animation
- Multiple content states
- Dynamic height adjustments
- Smooth transitions between states
- A toggle button with rotation animation

## Technical Details

- Built with react-native-reanimated for fluid animations
- Uses react-native-gesture-handler for touch interactions
- Implements worklet functions for native-thread performance
- Features spring animations for natural movement
- Supports custom styling and height configurations

## Implementation Notes

- Uses shared values for smooth state management
- Implements gesture clamping for controlled movements
- Provides ref-based control methods (open/close)
- Supports custom maximum height configuration
- Includes a backdrop component with fade animations

## Usage

```tsx
// Create a ref to control the trayconst ref = useRef<ActionTrayRef>(null);
// Open the trayref.current?.open();
// Close the trayref.current?.close();
// Check if tray is activeconst isActive = ref.current?.isActive();
```

GitHubAsk for support

Action Tray - FeedbackShare Your ThoughtsI value a lot your feedback! Help me improve by sharing your thoughts, suggestions, or reporting any issues you encounter. If you need assistance, send me an email at hello@reactiive.ioSend Feedback

---

*Documentation extracted from reactiive.io/demos*
