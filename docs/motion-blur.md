# Motion Blur

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/motion-blur)
> **Source Code**: [/src/animations/motion-blur](/src/animations/motion-blur)

## Tags
- `reanimated`
- `expo-blur`

## Description

Scan to try on your device

## Technical Implementation

- Blur animations
- Dynamic list rendering
- Item generation
- Visibility limiting
- Floating action button

## Usage

```typescript
// Data structuretype Item = {  id: number;  // Other item properties};
// Basic usage<BlurredList  data={items}  renderItem={({ item }) => <ListItem item={item} />}  maxVisibleItems={3}/>;
// Add new itemsconst addItem = () => {  setItems((prevItems) => [    ...prevItems,    generateRandomItem(prevItems.length + 1),  ]);};
// Add button<PressableScale onPress={addItem}>  <Entypo name="plus" size={40} color="white" /></PressableScale>;
```

---

*Documentation extracted from reactiive.io/demos*
