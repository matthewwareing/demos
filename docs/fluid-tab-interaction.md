# Fluid Tab Interaction

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/fluid-tab-interaction)
> **Source Code**: [/src/animations/fluid-tab-interaction](/src/animations/fluid-tab-interaction)

## Tags
- `reanimated`
- `expo-blur`

## Description

Scan to try on your device

## Usage

```tsx
import { SegmentedControl } from './components/segmented-control';
// Define your data structureconst data = [  { name: 'Accounts', icon: 'wallet-outline' },  { name: 'Deposits', icon: 'bank' },  { name: 'Funds', icon: 'chart-bar' },];
// Use the componentconst MyComponent = () => {  const [selected, setSelected] = useState(data[0]);  const { width } = useWindowDimensions();
  return (    <SegmentedControl      data={data}      onPress={setSelected}      selected={selected}      width={width - 40}      height={50}    />  );};
```

## Props

```typescript
type SegmentedControlProps<T extends { name: string; icon: string }> = {  data: readonly T[]; // Array of items to display in the control  onPress: (item: T) => void; // Callback function when an item is selected  selected: T; // Currently selected item  width: number; // Width of the control  height: number; // Height of the control};
```

---

*Documentation extracted from reactiive.io/demos*
