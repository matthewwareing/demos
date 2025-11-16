# Fluid Tab Interaction

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/fluid-tab-interaction)
> **Source Code**: [/src/animations/fluid-tab-interaction](/src/animations/fluid-tab-interaction)

## Tags
- `reanimated`
- `expo-blur`

## Usage

```tsx
import { SegmentedControl } from './components/segmented-control';
// Define your data structureconst data = [  { name: 'Accounts', icon: 'wallet-outline' },  { name: 'Deposits', icon: 'bank' },  { name: 'Funds', icon: 'chart-bar' },];
// Use the componentconst MyComponent = () => {  const [selected, setSelected] = useState(data[0]);  const { width } = useWindowDimensions();
  return (    <SegmentedControl      data={data}      onPress={setSelected}      selected={selected}      width={width - 40}      height={50}    />  );};
```

## Props

The SegmentedControl component accepts the following props:

```tsx
type SegmentedControlProps<T extends { name: string; icon: string }> = {  data: readonly T[]; // Array of items to display in the control  onPress: (item: T) => void; // Callback function when an item is selected  selected: T; // Currently selected item  width: number; // Width of the control  height: number; // Height of the control};
```

GitHubAsk for support

Fluid Tab Interaction - FeedbackShare Your ThoughtsI value a lot your feedback! Help me improve by sharing your thoughts, suggestions, or reporting any issues you encounter. If you need assistance, send me an email at hello@reactiive.ioSend Feedback

---

*Documentation extracted from reactiive.io/demos*
