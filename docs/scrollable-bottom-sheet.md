# Scrollable Bottom Sheet

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/scrollable-bottom-sheet)
> **Source Code**: [/src/animations/scrollable-bottom-sheet](/src/animations/scrollable-bottom-sheet)

## Tags
- `reanimated`
- `gesture-handler`

## What's This About?

This component creates an interactive bottom sheet that supports both vertical and horizontal scrolling between pages. Each page can have its own height and content, with smooth transitions between states. The implementation includes a gradient button trigger, page navigation controls, and programmatic scrolling methods, making it suitable for complex modal interfaces.

## Technical Implementation

The component uses:

- Multi-page navigation
- Vertical/horizontal scrolling
- Height management
- Gradient effects
- Ref-based control

## Usage

```tsx
// Page configurationconst pages = [  {    height: 350,    component: (      <BottomSheetPage        onPress={() => {          bottomSheetRef.current?.scrollToX(windowWidth);        }}        buttonTitle="Next Page"      />    ),  },  {    height: 500,    component: (      <BottomSheetPage        onPress={() => {          bottomSheetRef.current?.scrollToX(windowWidth * 2);        }}        buttonTitle="Next Page"      />    ),  },];
// Basic usage<ScrollableBottomSheet ref={bottomSheetRef} pages={pages} />;
// Control methodsbottomSheetRef.current?.scrollToY(-pageHeight);bottomSheetRef.current?.scrollToX(windowWidth);bottomSheetRef.current?.close();bottomSheetRef.current?.isActive();
```

GitHubAsk for support

Scrollable Bottom Sheet - FeedbackShare Your ThoughtsI value a lot your feedback! Help me improve by sharing your thoughts, suggestions, or reporting any issues you encounter. If you need assistance, send me an email at hello@reactiive.ioSend Feedback

---

*Documentation extracted from reactiive.io/demos*
