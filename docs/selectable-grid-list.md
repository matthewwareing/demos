# Selectable Grid List

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/selectable-grid-list)
> **Source Code**: [/src/animations/selectable-grid-list](/src/animations/selectable-grid-list)

## Tags
- `reanimated`
- `gesture-handler`

## What's This About?

This component creates an interactive grid list where items can be selected and deselected with animated transitions. It features a configurable grid layout, a floating action button that responds to selection state, and smooth animations for selection feedback. The implementation includes safe area handling and dynamic item sizing based on screen width, making it suitable for gallery or file selection interfaces.

## Technical Implementation

The component uses:

- Grid layout management
- Multi-selection handling
- Animated transitions
- Floating action button
- Safe area awareness

## Usage

```tsx
// Grid configurationconst GridConfig = {  itemsPerRow: 4,  internalPadding: 4,};
// Basic usage<SelectableGridList  data={items}  numColumns={GridConfig.itemsPerRow}  itemSize={itemSize}  onSelectionChange={(indexes) => {    selectedIndexesAmount.value = indexes.length;  }}  renderItem={({ index, activeIndexes }) => (    <SelectableListItem      index={index}      internalPadding={GridConfig.internalPadding}      containerWidth={itemSize}      containerHeight={itemSize}      activeIndexes={activeIndexes}    />  )}/>;
// Reset selectiongridListRef.current?.reset();
// Floating button animationconst rFloatingButtonStyle = useAnimatedStyle(() => {  return {    transform: [      {        translateY: withSpring(selectedIndexesAmount.value === 0 ? 150 : 0),      },    ],  };});
```

GitHubAsk for support

Selectable Grid List - FeedbackShare Your ThoughtsI value a lot your feedback! Help me improve by sharing your thoughts, suggestions, or reporting any issues you encounter. If you need assistance, send me an email at hello@reactiive.ioSend Feedback

---

*Documentation extracted from reactiive.io/demos*
