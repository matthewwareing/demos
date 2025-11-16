# Drag to Sort

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/drag-to-sort)
> **Source Code**: [/src/animations/drag-to-sort](/src/animations/drag-to-sort)

## Tags
- `reanimated`
- `gesture-handler`

## Description

Scan to try on your device

## What's This About?

- Items can be dragged to reorder
- Visual feedback shows current position
- Items adjust their shape while dragging
- Gradient overlay adds depth

## Technical Implementation

- Reanimated for drag gestures
- Custom list implementation for z-index handling
- Position tracking with shared values
- Linear gradient overlay
- Safe area handling

## Usage

```typescript
type Item = {  id: string;  title: string;  // other item properties};
// Basic usage<SortableList  data={items}  listItemHeight={80}  onDragEnd={(positions) => {    console.log('New order:', positions);  }}  renderItem={({ item, index }) => (    <ListItem      item={item}      index={index}      style={{        height: 80,        margin: 6,      }}    />  )}/>;
```

---

*Documentation extracted from reactiive.io/demos*
