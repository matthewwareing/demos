# Theme Canvas Animation

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/theme-canvas-animation)
> **Source Code**: [/src/animations/theme-canvas-animation](/src/animations/theme-canvas-animation)

## Tags
- `skia`

## Description

Scan to try on your device

## Technical Implementation

- Skia canvas
- Circular animations
- Theme management
- Custom fonts
- Gesture handling

## Usage

```typescript
// Basic usage<ThemeCanvasAnimation />;
// Theme configurationconst colors = [  { background: '#F7FFF7', text: '#373737' },  { background: '#4ECDC4', text: '#2C2C2C' },  { background: '#1A535C', text: '#E8E8E8' },  { background: '#EE6C4D', text: '#D4D2D2' },  { background: '#F38D68', text: '#2C2C2C' },  { background: '#902D41', text: '#DEDEDE' },];
// Square coordinates calculationconst coordinates = useDerivedValue(() => {  const squares = [    { offsetX: -1, offsetY: 0 },    { offsetX: 0, offsetY: 0 },    { offsetX: 1, offsetY: 0 },    { offsetX: 0, offsetY: 1 },    { offsetX: -1, offsetY: 1 },    { offsetX: 1, offsetY: 1 },  ];
  return squares.map(({ offsetX, offsetY }) => ({    cx: canvasWidth / 2 - SQUARE_SIZE / 2 + offsetX * SQUARE_SIZE * 2,    cy: canvasHeight / 2 - SQUARE_SIZE / 2 + offsetY * SQUARE_SIZE * 2,  }));}, [canvasWidth, canvasHeight]);
// Theme transitionconst onSelectSquare = (index: number) => {  radius.value = withTiming(canvasHeight, {    duration: 500,  });  previousSelectedIndex.value = selectedIndex.value;  selectedIndex.value = index;};
```

---

*Documentation extracted from reactiive.io/demos*
