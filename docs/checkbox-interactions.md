# Checkbox Interactions

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/checkbox-interactions)
> **Source Code**: [/src/animations/checkbox-interactions](/src/animations/checkbox-interactions)

## Tags
- `reanimated`

## What's This About?

This component creates an interactive checkbox interface for selecting favorite cuisines. Each checkbox features smooth animations for selection and deselection, with a modern design that provides clear visual feedback for user interactions.

## Technical Implementation

The component implements:

- Custom checkbox animations
- Safe area handling for proper layout
- Flexible grid layout for multiple options
- State management for selections
- Typography and spacing optimizations

## Usage

```tsx
type Cuisine = {  id: string;  name: string;  selected: boolean;};
// Basic checkbox usage<Checkbox label="Italian" checked={isSelected} onPress={handleSelection} />;
// Full implementationconst { cuisines, toggleCuisine } = useCuisines();
<View>  {cuisines.map((cuisine) => (    <Checkbox      key={cuisine.id}      label={cuisine.name}      checked={cuisine.selected}      onPress={() => toggleCuisine(cuisine.id)}    />  ))}</View>;
```

GitHubAsk for support

Checkbox Interactions - FeedbackShare Your ThoughtsI value a lot your feedback! Help me improve by sharing your thoughts, suggestions, or reporting any issues you encounter. If you need assistance, send me an email at hello@reactiive.ioSend Feedback

---

*Documentation extracted from reactiive.io/demos*
