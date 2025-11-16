# Selectable Grid List

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/selectable-grid-list)
> **Source Code**: [/src/animations/selectable-grid-list](/src/animations/selectable-grid-list)

## Tags
- `reanimated`
- `gesture-handler`

## Description

Scan to try on your device

## Technical Implementation

- Grid layout management
- Multi-selection handling
- Animated transitions
- Floating action button
- Safe area awareness

## Usage

```typescript
// Grid configurationconst GridConfig = {  itemsPerRow: 4,  internalPadding: 4,};
// Basic usage<SelectableGridList  data={items}  numColumns={GridConfig.itemsPerRow}  itemSize={itemSize}  onSelectionChange={(indexes) => {    selectedIndexesAmount.value = indexes.length;  }}  renderItem={({ index, activeIndexes }) => (    <SelectableListItem      index={index}      internalPadding={GridConfig.internalPadding}      containerWidth={itemSize}      containerHeight={itemSize}      activeIndexes={activeIndexes}    />  )}/>;
// Reset selectiongridListRef.current?.reset();
// Floating button animationconst rFloatingButtonStyle = useAnimatedStyle(() => {  return {    transform: [      {        translateY: withSpring(selectedIndexesAmount.value === 0 ? 150 : 0),      },    ],  };});
```

---

*Documentation extracted from reactiive.io/demos*
