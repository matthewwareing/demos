# Draggable Panel

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/draggable-panel)
> **Source Code**: [/src/animations/draggable-panel](/src/animations/draggable-panel)

## Tags
- `reanimated`
- `gesture-handler`
- `react-native`

## Description

Scan to try on your device

## The code structure

```typescript
src/├── components/│   ├── draggable-panel/│   │   └── draggable-control-panel.tsx  # The main draggable logic│   └── spring-animation-panel/│       ├── index.tsx                     # Manages spring states│       ├── panel-content.tsx             # The UI for spring selection│       └── collapsed-button.tsx          # That little settings icon└── index.tsx                             # Entry point
```

## Want to use it?

```tsx
import { DraggableControlPanel } from './components/draggable-panel/draggable-control-panel';import { useSharedValue } from 'react-native-reanimated';
function App() {  return (    <View style={{ flex: 1 }}>      {/* Your app goes here */}      <DraggableControlPanel        springConfig={{          damping: 30,          stiffness: 200,        }}        collapsedChildren={(toggleCollapse) => (          <Pressable onPress={toggleCollapse}>            <Text>👆</Text>          </Pressable>        )}        expandedChildren={(toggleCollapse) => (          <View>            <Text>Your expanded content here</Text>            <Button onPress={toggleCollapse} title="Collapse" />          </View>        )}        collapsedWidth={64}        collapsedHeight={64}        expandedWidth={280}        expandedHeight={150}      />    </View>  );}
```

---

*Documentation extracted from reactiive.io/demos*
