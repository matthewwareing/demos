# Scrollable Bottom Sheet

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/scrollable-bottom-sheet)
> **Source Code**: [/src/animations/scrollable-bottom-sheet](/src/animations/scrollable-bottom-sheet)

## Tags
- `reanimated`
- `gesture-handler`

## Description

Scan to try on your device

## Technical Implementation

- Multi-page navigation
- Vertical/horizontal scrolling
- Height management
- Gradient effects
- Ref-based control

## Usage

```typescript
// Page configurationconst pages = [  {    height: 350,    component: (      <BottomSheetPage        onPress={() => {          bottomSheetRef.current?.scrollToX(windowWidth);        }}        buttonTitle="Next Page"      />    ),  },  {    height: 500,    component: (      <BottomSheetPage        onPress={() => {          bottomSheetRef.current?.scrollToX(windowWidth * 2);        }}        buttonTitle="Next Page"      />    ),  },];
// Basic usage<ScrollableBottomSheet ref={bottomSheetRef} pages={pages} />;
// Control methodsbottomSheetRef.current?.scrollToY(-pageHeight);bottomSheetRef.current?.scrollToX(windowWidth);bottomSheetRef.current?.close();bottomSheetRef.current?.isActive();
```

---

*Documentation extracted from reactiive.io/demos*
