# Checkbox Interactions

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/checkbox-interactions)
> **Source Code**: [/src/animations/checkbox-interactions](/src/animations/checkbox-interactions)

## Tags
- `reanimated`

## Description

Scan to try on your device

## Technical Implementation

- Custom checkbox animations
- Safe area handling for proper layout
- Flexible grid layout for multiple options
- State management for selections
- Typography and spacing optimizations

## Usage

```typescript
type Cuisine = {  id: string;  name: string;  selected: boolean;};
// Basic checkbox usage<Checkbox label="Italian" checked={isSelected} onPress={handleSelection} />;
// Full implementationconst { cuisines, toggleCuisine } = useCuisines();
<View>  {cuisines.map((cuisine) => (    <Checkbox      key={cuisine.id}      label={cuisine.name}      checked={cuisine.selected}      onPress={() => toggleCuisine(cuisine.id)}    />  ))}</View>;
```

---

*Documentation extracted from reactiive.io/demos*
