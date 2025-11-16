# Motion Blur

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/motion-blur)
> **Source Code**: [/src/animations/motion-blur](/src/animations/motion-blur)

## Tags
- `reanimated`
- `expo-blur`

## What's This About?

This component creates a dynamic list interface with a sophisticated motion blur effect. When new items are added to the list, they appear with a smooth blur animation that enhances the sense of motion and depth. The component includes a floating action button for adding items and limits the number of visible items to maintain performance while preserving the visual effect.

## Technical Implementation

The component uses:

- Blur animations
- Dynamic list rendering
- Item generation
- Visibility limiting
- Floating action button

## Usage

```tsx
// Data structuretype Item = {  id: number;  // Other item properties};
// Basic usage<BlurredList  data={items}  renderItem={({ item }) => <ListItem item={item} />}  maxVisibleItems={3}/>;
// Add new itemsconst addItem = () => {  setItems((prevItems) => [    ...prevItems,    generateRandomItem(prevItems.length + 1),  ]);};
// Add button<PressableScale onPress={addItem}>  <Entypo name="plus" size={40} color="white" /></PressableScale>;
```

GitHubAsk for support

Motion Blur - FeedbackShare Your ThoughtsI value a lot your feedback! Help me improve by sharing your thoughts, suggestions, or reporting any issues you encounter. If you need assistance, send me an email at hello@reactiive.ioSend Feedback

---

*Documentation extracted from reactiive.io/demos*
